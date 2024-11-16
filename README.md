# variable-service
Variable service to handle multiple env loaders and parsers
## Initial TODO/Ideas 
 - parser need to have link to type import?
 - build cli tool to add/remove custom parsers to JSON (we need to have type name someways if build custom type for this)
 - build cli tool to add/remove variable name and parser (in namespace) on JSON
   - make interactive (ask name, ask parser, ask namespace, ask if have default value, ask if like to throw error if not found (else creates T| undefined)
 - have namespaces (and default namespace)
 - on startup register all parsers and throw error if not have custom parser types registered on JSON.
 - store variable json file location to package.json?
 - build automatically variable key type file based on JSON? (if touch with cli or in "watch" mode, check how to drop this on code? push node_module or other ways?)


## code usage ideas
```typescript
const port: string = varSrv.useNS('web').get('PORT');
const db: URL = varSrv.useDefaultNS().get('DB');
```
