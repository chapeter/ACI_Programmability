###Example 2
Example 3 tier app creation using SDK

```python
from cobra.model.fv import *from cobra.model.pol import UniuniMo = Uni('')t = Tenant(uniMo, 'Tenant1')ap = Ap(t, 'Exchange')epg1 = AEPg(ap, 'OWA')epg2 = AEPg(ap, 'FrontEnd')epg3 = AEPg(ap, 'MailBox')ep = RsPathAtt(epg1, tDn=‘topology/pod-1/paths-17/paths-[eth1/1]’, mode=‘regular’, encap=‘vlan-10’)c = ConfigRequest()c.addMo(t)moDir.commit(c)
```

