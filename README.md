# Como Alterar o Arquivo Hosts

O arquivo `hosts` mapeia manualmente nomes de domínio para IPs.  
Formato:
```
<IP> <domínio>
```
Exemplo:
```
127.0.0.1 meuapp.local
```

---

## Ubuntu / Linux
1. Editar:
```bash
sudo nano /etc/hosts
```
2. Adicionar entrada e salvar (**CTRL+O**, **Enter**, **CTRL+X**).

---

## macOS
1. Editar:
```bash
sudo nano /etc/hosts
```
2. Limpar cache:
```bash
sudo dscacheutil -flushcache && sudo killall -HUP mDNSResponder
```

---

## Windows
1. Abrir **Bloco de Notas como administrador**.  
2. Abrir arquivo:
```
C:\Windows\System32\drivers\etc\hosts
```
3. Alterar filtro para "Todos os arquivos" e salvar mudanças.

---

## Testar
```bash
ping meuapp.local
```
Ou:
```
http://meuapp.local
```
