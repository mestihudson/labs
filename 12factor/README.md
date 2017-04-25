# 12 Factor Application (Doze Fatores de uma Aplicação)

Hoje, muitas aplicações são serviços implantados na nuvem, na infra-estrutura provida por empresas tais como Amazon AWS, Google Compute Engine, DigitalOcean, Rackspace, OVH, ...

Heroku é uma PaaS (Platform as a Service - Plataforma com um Serviço) que confia na nuvem da Amazon AWS e que faz a implantação de aplicações tão fácil quanto um  `git push heroku master` (executado a partir da raiz de sua aplicação).

Com um grande número de aplicações implantadas no Heroku, engenheiros da companhia adiquiriram grande conhecimento do que deve ser feito para tornar uma aplicação nativa  disponível na nuvem.

A metodologia 12 fatores (12 factor) é resultado das observações deles. Como nomes de estados, ele apresenta 12 princípios que irão ajudar a aplicação a estar ápita para a nuvem, horizontalmente escalável, e portável.

# Organisation of this lab

In this lab, we will start by building a simple Node.js application as an HTTP Rest API exposing CRUD (Create / Read / Update / Delete) verbs on a *message* model.

HTTP verb | URI | Action
----------| --- | ------
GET | /message | list all messages
GET | /message/ID | get message with ID
POST | /message | create a message user
PUT | /message/ID | modify message with ID
DELETE | /message/ID | delete message with ID

We will then follow each one of the 12 factor and see how this can leverage our application. At the same time, we will see that Docker is a really great fit for several of those factors.

# Let's get started !

[Build the application](00_application.md)

[1 - Codebase](01_codebase.md)

[2 - Dependencies](02_dependencies.md)

[3 - Configuration](03_configuration.md)

[4 - External services](04_external_services.md)

[5 - Build / Release / Run](05_build_release_run.md)

[6 - Processes](06_processes.md)

[7 - Port binding](07_port_binding.md)

[8 - Concurrency](08_concurrency.md)

[9 - Disposability](09_disposability.md)

[10 - Dev / Prod parity](10_dev_prod_parity.md)

[11 - Logs](11_logs.md)

[12 - Admin processes](12_admin_processes.md)

Do not hesitate to provide comments / feedback you may have in order to improve this lab.
