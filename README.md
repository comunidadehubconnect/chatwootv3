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

```bash
systemctl daemon-reload && systemctl restart chatwoot.target
```

### Caso sua recompilação falhe ou encontre algum erro `ActionView::Template::Error (Webpacker can't find application.css in /home/chatwoot/chatwoot/public/packs/manifest.json)` ou qualquer outro erro, basta executar o comando abaixo:

```bash
RAILS_ENV=production rake assets:clean assets:clobber assets:precompile
```

Observação: Este comando limpará os ativos compilados existentes e recompilará todos os ativos. [Leia mais sobre isso aqui].
(https://edgeguides.rubyonrails.org/command_line.html#bin-rails-assets)

<hr />
<hr />
