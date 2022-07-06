# Resource Group commands

## list based on name

Get ID within a column

```bash
query_string='ala'
az group list --query "[?contains(name, '$query_string')].[id]" --output table
```

Return only ID
```bash
query_string='ala'
az group list --query "[?contains(name, '$query_string')].[id]" --output tsv
```