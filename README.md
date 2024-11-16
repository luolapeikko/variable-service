# variable-service
Variable service to handle multiple env loaders and parsers
## Initial TODO/Ideas
 - build cli tool to add/remove custom parsers to JSON
 - build cli tool to add/remove variable name and parser (in namespace) on JSON
 - have namespaces (and default namespace)
 - on startup register all parsers and error if not have custom parser types registered on JSON.
 - store variable json file location to package.json?
 - build automatically variable key type file based on JSON? (if touch with cli or in "watch" mode, check how to drop this on code? push node_module or other ways?)
