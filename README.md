# config

-Powershell Command:
Invoke-RestMethod -Method Post -Uri http://localhost:7171/actuator/refresh -Body '{}' -ContentType "application/json"

-Extra:
$headers = @{
  Authorization = 'Basic Yw...='
}
Invoke-RestMethod -Method Post -Uri https://dnsadmin.test.com/apikeys -Headers $headers -ContentType "application/json" -Body '{"description": "masterkey","domains":["testapi.com"], "role": "User"}'
