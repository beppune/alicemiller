```
on confirm log request
on revoke {
	log "La richiesta ${req.id} è stata revocata"
	mailto marchis6 {
		subject "Revoca rihiesta ${req.id}"
		body "La richiesta ${req.id} è stata revocata da ${op.uid}."
	}
}

on submit validate ok
on submit
	validate "Nessuna richiesta di accesso a RM2 nei il 12 maggio causa lavori"
	ko {
		req.location == 'RM2', req.start_date == '12/05/2025'.
		
		log "Validazione fallita: ${summary}"
	}
```

### Grammar

SPEC := EVENT_SPEC
EVENT_SPEC := 'on' EVENT_NAME SPEC_DEFINITION
EVENT_NAME : 'confirm'|'revoke'|'submit'
SPEC_DEFINITION := COMMAND '\n' | { COMMAND_LIST }