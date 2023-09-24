<p align="center">
<img src="https://cwmkt.com.br/wp-content/uploads/2023/08/logo-github-cwmkt.svg" alt="DispZap Whats Marketing" width="240" />
<p align="center">Seja bem-vindo ao Guia de atualização de como atualizar versão V3 do Chatwoot🚀</p>
</p>
  
<p align="center">
<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
<span>Grupo WhatsaAPP: </span>
<a href="https://link.cwmkt.com.br/grupo-whats" target="_blank">Grupo</a>
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

