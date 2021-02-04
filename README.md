# WAF-Hook

WAF-Hook é um software pequeno desenvolvido para a detecção de sistemas de proteção, CDN (Content Delivery Network) e balanceadores para websites.
Baseado em análises de requisições a websites, este aplicativo determina a proteção que determinado website analisado está a utilizar.
Atualmente o aplicativo está em fase inicial de desenvolvimento, portanto, não detectando em sua totalidade uma grande quantidade de WAF´s.
Este aplicativo é mantido pela XLabs Security, uma empresa de Segurança Web que irá manter a base e a aplicação atualizadas.

WAF-Hook is a small software developed for the detection of protection systems, CDN (Content Delivery Network) and balancers for websites.
Based on analysis of requests to websites, this application determines the protection that a website analyzed is using.
Currently the application is in the early stages of development, therefore, it does not fully detect a large amount of WAFs.
This application is maintained by XLabs Security, a web security company that will keep the database and application up to date.


O **App Mobile WAF-Hook** inicialmente foi desenvolvido para Android em suas novas versões,
desenvolvido para a detecção de Web Application Firewalls e outras plataformas de defesa para aplicações web

https://play.google.com/store/apps/details?id=br.com.wafhook


## Um pouco sobre o funcionamento do app WAF-Hook

O WAF-Hook possui duas formas de detecção de WAFs ou alguns Firewalls de Nova Geração (NGFW) que possuam filtros Web.

- **Detecção Passiva**:
O WAF-Hook utilizando as conexões do mobile, efetua um acesso normal ao website,
analisando cabeçalhos da comunicação HTTP/HTTPS ele pode determinar através de assinaturas
a presença de WAFs ou NGFWs protegendo aplicações web.


- **Detecção Ativa**:
O WAF-Hook utilizando as conexões do mobile, efetua acessos anormais, 
acessos estes característicos de ataques a aplicações web, tendo como objetivo não a exploração da aplicação web,
e sim fazer com que o sistema de defesa da aplicação web demonstre suas telas de bloqueio ou então informações em cabeçalhos
durante o bloqueio da requisição efetuada.


- **Detecção Hibrida**:
O WAF-Hook utiliza primeiro a verificação passiva e logo após efetua a verificação ativa


A seguir as assinaturas de WAFs já catalogados e presentes na atual Database

## WAF/CDN da XLabs Security

- Forma de detecção: **Passiva**; 


## WAF/CDN da CloudFlare

- Forma de detecção: **Passiva**; 


## WAF ou ELB da Amazon Cloudfront

- Forma de detecção: **Passiva**; 


## WAF da Sucuri CloudProxy

- Forma de detecção: **Passiva**; 


## WAF/CDN da Imperva Incapsula

- Forma de detecção: **Hibrida**; 


## WAF da YxLink

- Forma de detecção: **Passiva**; 


## WAF da ArvanCloud

- Forma de detecção: **Passiva**; 


## WAF da DoSArrest Internet Security

- Forma de detecção: **Passiva**; 


## WAF/CDN da Akamai KONA Site Defender

- Forma de detecção: **Passiva**; 


## WAF da Fortinet Fortigate WAF (Appliance)

- Forma de detecção: **Ativa**; 


## WAF NAXSI

- Forma de detecção: **Hibrida**; 


## WAF da Citrix NetScaler AppFirewall

- Forma de detecção: **Passiva**; 


## WAF da Wordfence (Plugin para Wordpress)

- Forma de detecção: **Ativa**; 


## WAF da Radware (Radware Appwall)

- Forma de detecção: **Ativa**; 


## WAF da Cisco (Cisco ACE XML Gateway)

- Forma de detecção: **Passiva**; 


## WAF da BIG-IP AppSec Manager (F5 Networks)

- Forma de detecção: **Ativa**;


### Não encontrou o WAF nesta lista?
Não fique triste, compartilhe conosco as formas de detecções enviando um email para dev@xlabs.com.br
