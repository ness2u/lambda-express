# express on lambda
this is about the simplist setup to prove its possible.


# deploy + cleanup
`./package` will zip/push things to s3
`./deploy` creates the lambda functions
`./delete-stack` will remove the stack

# api-gateway config
This was done manually.

- Create a new api
- Create a new resource for `/`
- Create a new method for `Any`, point it at the lambda function.
- Deploy the API, which will provide the URI for hitting the service.
