###Example 1
Example Tenant Creation using SDK

```python
from cobra.model.fv import Tenant
from cobra.model.pol import Uni
from cobra.mit.request import ConfigRequest
uniMo = Uni('')  # Uni is a static Mo, so we don’t need to look it up
t = Tenant(uniMo, 'Tenant1')  # We create a tenant as a child of the universe
c = ConfigRequest()  # Create a ConfigRequest to contain our new object
c.addMo(t)  # Add our tenant to the ConfigRequest
moDir.commit(c)  # Commit our configuration request
```

