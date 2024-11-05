bash``` 
-- vscode :: launch.json 
{
    "configurations": [
        {
            "name": "basic asset transfer",
            "type": "hlf-go",
            "request": "launch",
            "isCaas": false
        }
    ]
}
```

```
-- testing with chaincode ===> (test.fabric)
[
    {
        "query":"GetAllAssets",
        "args":[]
    }
    ,{
        "invoke": "InitLedger", 
        "args": []
    },
    {
        // id string,
        //  color string, 
        //  size int, 
        //  owner string,
        //   appraisedValue int
        
        "invoke":"CreateAsset",
        "args":[
            "asset111",
            "yallow",
            20,
            "king",
            200
        ]
    }
]

```