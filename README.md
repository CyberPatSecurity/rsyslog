# Configurazione Syslog Server per ricezione log Fortinet (CEF → Sentinel)

## 🔧 Dettagli macchina

- Hostname: `SyslogServer`
- IP: `10.160.99.41`
- Sistema: Rocky Linux 9
- Utente amministratore: `sentinelAdmin`

---

## 🔐 Firewall (firewalld)

```bash
sudo firewall-cmd --permanent --add-port=514/udp
sudo firewall-cmd --permanent --add-port=514/tcp
sudo firewall-cmd --reload

