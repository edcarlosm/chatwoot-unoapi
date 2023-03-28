# chatwoot-unoapi
 Chatwoot com a unoapi
 </p></p>
Para testar o chatwoot com a unoapi você tera que ter o docker instalado.
<p>
curl -L https://get.docker.com | sh
</p>
adicionar seu usuario ao grupo docker isso se você não estiver utilizando root
</p>
sudo usermod -aG docker $USER 
</p>
Download dos seguintes arquivos
</p>
wget https://github.com/edcarlosm/chatwoot-unoapi/blob/main/unoapi.tar.gz
</p>
wget https://github.com/edcarlosm/chatwoot-unoapi/blob/main/chatwoot.tar.gz
</p>
extraia os dois arquivos chatwoot e uno api
</p>
tar -xzvf unoapi.tar.gz
</p>
tar -xzvf chatwoot.tar.gz
</p>
edite o .env com o ip da sua vps. recomendo não utilizar em produção mais se quiser é só coloca o endereço do seu chatwoot.
</p>
crie uma rede para ser utilizada pelo docker, rode o comando a baixo no seu terminal.
</p>
docker network create --subnet=172.18.0.0/16 kabacorp
</p>
entre na pasta chatwoot que foi extraida e de o seguinte comando.
</p>
docker compose pull
</p>
docker compose up -d
</p>
entre na pasta uno que foi extraida e de o seguinte comando.
</p>
docker compose pull
</p>
docker compose up -d
</p>
acesse o ip:3000 ou endereço se você fez todos os procedimentos para utilizar o dominio.
</p>
login e senha para acesso
</p>
edcarlos@kabaweb.in
Kabacorp2023@
</p>
adicione sua caixa de entrada e pode testa a uno api via docker.
</p>
Não remomendo utilizar em produção. materia só para testes mesmo e demostração da eficiencia da unoapi
</p>
se gostou e quiser contribuir com um pix deixei meu qrcode na parte da logo do chatwoot. 
