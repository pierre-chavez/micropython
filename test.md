# Titulo 
## Titulo 2
### Titulo 3

```markdown
import smtplib

fromAddr = 'pierre_chavez@icloud.com'
toAddr = ['pierre_chavez@outlook.com']
subject = 'test'
smtpServer = 'smtp.mail.me.com:587'

#f = open('mensaje.txt', 'r')
msg = 'hola pierre'
#f.close()

header = 'From: %s\r\n' % fromAddr
header += 'To: %s\r\n' % toAddr


msg = header + msg

try: 
	server = smtplib.SMTP("smtp.mail.me.com",587)
	server.starttls()
	server.login('pierre_chavez@icloud.com','qtpx-wmzf-glig-qwkz')
	server.sendmail(fromAddr,toAddr,msg)
	server.quit()
	print('mensaje enviado correctamente\n')
except Exception as e:
	print('mensaje no enviado ', e)

```

- [x] opcion 1
- [ ]	opcion 2
- [ ]	opcion 3
