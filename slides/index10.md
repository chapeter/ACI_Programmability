###Example of creating a Tenant in the GUI
![](https://github.com/chapeter/ACI_Programmability_Intro/tree/master/images/aci-api-inspector-3.png)

We can see the interesting code here:

```json
method: POST
url: http://10.94.238.68/api/node/mo/uni.json
payload{"polUni":{"attributes":{"dn":"uni","status":"modified"},"children":[{"fvTenant":{"attributes":{"dn":"uni/tn-imapex101","status":"deleted"},"children":[]}}]}}
response: {"totalCount":"0","imdata":[]}
```

