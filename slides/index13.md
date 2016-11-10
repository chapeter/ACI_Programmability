###Authentication
The SDK takes care of staying logged into the fabric for you.  Example code to handle login and session.

```python
import cobra.mit.access
import cobra.mit.session

APIC_URL = 'http://<APIC_IP>'
APIC_USERNAME = 'username'
APIC_PASSWORD = 'password'

ls = cobra.mit.session.LoginSession(APIC_URL, APIC_USERNAME, APIC_PASSWORD)

md = cobra.mit.access.MoDirectory(ls)

md.login()
```

