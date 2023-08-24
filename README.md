<p align="center">
	<img src="https://www.chatwoot.com/docs/img/logo.png" alt="Chatwoot-logo" width="100" />	
	<p align="center">O Chatwoot oferece todas as ferramentas para gerenciar conversas, construir relacionamentos e encantar seus clientes em um só lugar.</p>
</p>

<p align="left">
	<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
	<span>Grupo WhatsaAPP: </span>
	<a href="https://chat.whatsapp.com/CLKge3hmHmmBcIL04mBzmT" target="_blank">Grupo</a>
</p>

<hr />
<hr />

**Como atualizar Chatwoot V3**

```bash
sudo cwctl --upgrade
```

<hr />
<hr />

**Como atualizar Chatwoot V3 Manualmente**


### Caso esteja usando node 18 precisa ser migrado para 16 depois retornado para 18.

```bash
sudo apt-get remove nodejs -y
```

```bash
sudo apt-get purge nodejs
```

```bash
sudo apt-get autoremove
```

```bash
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
```

```bash
sudo apt-get install -y nodejs
```

### Chatwoot

```bash
sudo -i -u chatwoot
```

```bash
cd chatwoot
```

```bash
git checkout master
```

```bash
git pull
```

Caso apareça a mensagem abaixo, basta digitar o seguinte comando:

```bash
git stash
```

![image](https://github.com/cwmkt/chatwootv3/assets/34479816/4c707ea5-b39f-4a4c-922d-bb4a5f959c59)


```bash
bundle
```

```bash
yarn
```

```bash
rake assets:precompile RAILS_ENV=production
```

```bash
RAILS_ENV=production bundle exec rake db:migrate
```

```bash
exit
```

```bash
systemctl daemon-reload && systemctl restart chatwoot.target
```

### Voltando para versão node 18

```bash
sudo apt-get remove nodejs
```

```bash
sudo apt-get purge nodejs
```

```bash
sudo apt-get autoremove
```

```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
```

```bash
sudo apt-get install -y nodejs
```

<hr />
<hr />
