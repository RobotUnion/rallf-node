# rallf-node

rallf-node must implement an API in order to bind to rallf-network

## API Documentation

### Node info (version, os, software, etc)
`GET` `/api/v1.0/info`
```
{
  "devices": [
    {
      "os": "linux",
      "program": "chromium"
    }
  ],
  "status": "ready",
  "version": "1.0.0-alpha1"
}
```

### Node executions (creates new execution in the node)
`POST` `/api/v1.0/executions`
  * `execution_id` `string` `required`
  * `package` `string` `required`
  * `input` `json` `optional`
  * `robot` `json` `optional`

```
{
  "status": "ok"
}
```
