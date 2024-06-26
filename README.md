# FlaskApp

Foi utilizado o GCP para deployar a aplicação do Flask.

O processo de pipeline automatizada consiste em, qualquer atualização efetuada no repositório (GitHub), ele deploya a aplicação em um Cloud Run do GCP, através de uma pipeline criada no Cloud Build do GCP.

## Cloud Run

Foi escolhido pelo baixo nível de complexidade, por ser serverless e ter opções de rolling update, escalabilidade e alta disponibilidade. Através do Cloud Run é possível coletar logs da aplicação e ter métricas de recursos, redes, etc., além de vantagens em termos de custo.

## Cloud Build

Foi escolhida esta ferramenta de pipeline pela fácil integração com os serviços do Google, diminuindo o overhead de implementação e garantindo compatibilidade com diversos tipos de repositório.

## Aplicação `comment.py`

Efetuei a containerização da aplicação para rodar no Cloud Run.

## Desenho da Arquitetura

![Desenho da Arquitetura]
