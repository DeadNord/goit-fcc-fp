# goit-fcc-fp

# FP‑App — Static Nginx Demo

Це демо‑проєкт для фінального завдання (Elastic Beanstalk + Docker).  
Запускає офіційний образ **nginx:1.27‑alpine** без додаткового коду.

## Швидкий старт

```bash
# 1. Ініціалізуємо EB (використовуючи існуючий .elasticbeanstalk/)
eb init

# 2. Створюємо середовище
eb create fp-prod-env --vpc.id <VPC_ID> --vpc.ec2subnets <SUBNET_PUB1>,<SUBNET_PUB2> --vpc.publicip

# 3. Деплой (після змін Dockerrun чи конфігу)
eb deploy

# 4. Відкрити у браузері
eb open

# Для видаленя
eb terminate fp-prod-env --profile fp-deployer
