# UFW Command Reference

| Purpose | Command |
|---|---|
| Allow SSH | `sudo ufw allow ssh` |
| Deny incoming traffic by default | `sudo ufw default deny incoming` |
| Allow outgoing traffic by default | `sudo ufw default allow outgoing` |
| Enable the firewall | `sudo ufw enable` |
| Allow the web port | `sudo ufw allow 8080/tcp` |
| Display detailed status | `sudo ufw status verbose` |
| Display numbered rules | `sudo ufw status numbered` |
| Test the web application | `curl http://localhost:8080` |

## Configuration Explanation

SSH is allowed before enabling UFW to preserve remote administration access. The Default Deny policy blocks incoming traffic unless an explicit rule permits it. Port 8080 is opened for TCP connections so users can access the deployed web application.

## Security Warning

If UFW is enabled before an SSH allow rule is added, incoming SSH connections may be blocked and remote access to the server may be lost.
