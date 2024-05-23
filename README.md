<p align="center">
<img src="https://cwmkt.com.br/wp-content/uploads/2024/04/logo_github.png" width="240" />
<p align="center">Seja bem-vindo ao Guia de atualização de como atualizar versão V3 do Chatwoot🚀</p>
</p>
  
<p align="center"> 
<a href="https://hubconnect.top" target="_blank">👉 Participe da Comunidade HubConnect 👈</a>
</p>

<hr />
<hr />

**Como atualizar Chatwoot V3**

```bash
sudo cwctl --upgrade
```

<hr />
<hr />

### Como atualizar Chatwoot V3 Manualmente



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

### Copie os novos arquivos atualizados

```bash
cp /home/chatwoot/chatwoot/deployment/chatwoot-web.1.service /etc/systemd/system/chatwoot-web.1.service
cp /home/chatwoot/chatwoot/deployment/chatwoot-worker.1.service /etc/systemd/system/chatwoot-worker.1.service
cp /home/chatwoot/chatwoot/deployment/chatwoot.target /etc/systemd/system/chatwoot.target
```

```bash
systemctl daemon-reload && systemctl restart chatwoot.target
```

