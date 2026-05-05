# R3 Rental Car - Fotos da Frota

Repositorio publico com fotos da frota da R3 Rental Car organizadas por categoria e modelo.
Bot do WhatsApp consome essas fotos para enviar quando cliente pedir.

## Estrutura

- Cada categoria tem sua pasta
- Dentro da categoria, cada modelo tem sub-pasta
- Fotos genericas da categoria ficam direto na pasta da categoria
- manifest.json na raiz lista as URLs ativas

## Categorias

### Sedan Mid Size
- Pasta: [sedan-mid-size/](./sedan-mid-size/)
- HQ vehicle_class_id: 3
- Modelos:
  - [Toyota Corolla](./sedan-mid-size/toyota-corolla/)
  - [Toyota Camry](./sedan-mid-size/toyota-camry/)
  - [Hyundai Accent](./sedan-mid-size/hyundai-accent/)
  - [Buick Verano](./sedan-mid-size/buick-verano/)
  - [Dodge Dart](./sedan-mid-size/dodge-dart/)
  - [Kia Forte](./sedan-mid-size/kia-forte/)
  - [Kia Optima](./sedan-mid-size/kia-optima/)
  - [Ford Fusion](./sedan-mid-size/ford-fusion/)

### SUV Midsize (Standard)
- Pasta: [suv-midsize/](./suv-midsize/)
- HQ vehicle_class_id: 8
- Modelos:
  - [Hyundai Santa Fe](./suv-midsize/hyundai-santa-fe/)
  - [Honda Odyssey](./suv-midsize/honda-odyssey/)
  - [Jeep Cherokee](./suv-midsize/jeep-cherokee/)
  - [Ford Ecosport](./suv-midsize/ford-ecosport/)
  - [Kia Sportage](./suv-midsize/kia-sportage/)
  - [Vw Taos](./suv-midsize/vw-taos/)

### SUV Premium
- Pasta: [suv-premium/](./suv-premium/)
- HQ vehicle_class_id: 5
- Modelos:
  - [Vw Atlas](./suv-premium/vw-atlas/)
  - [Vw Tiguan](./suv-premium/vw-tiguan/)
  - [Hyundai Santa Fe](./suv-premium/hyundai-santa-fe/)
  - [Dodge Durango](./suv-premium/dodge-durango/)
  - [Jeep Grand Cherokee](./suv-premium/jeep-grand-cherokee/)
  - [Bmw X1](./suv-premium/bmw-x1/)

### Minivan 7 lugares
- Pasta: [minivan-7-lugares/](./minivan-7-lugares/)
- HQ vehicle_class_id: 1
- Modelos:
  - [Kia Sedona](./minivan-7-lugares/kia-sedona/)
  - [Chrysler Pacifica](./minivan-7-lugares/chrysler-pacifica/)
  - [Chrysler Voyager](./minivan-7-lugares/chrysler-voyager/)

### Minivan 8 lugares
- Pasta: [minivan-8-lugares/](./minivan-8-lugares/)
- HQ vehicle_class_id: 15
- Modelos:
  - [Kia Sedona 8 Lugares](./minivan-8-lugares/kia-sedona-8-lugares/)
  - [Chrysler Pacifica 8 Lugares](./minivan-8-lugares/chrysler-pacifica-8-lugares/)

### SUV Full Size Luxo (7-8 lugares Premium)
- Pasta: [suv-full-size-luxo/](./suv-full-size-luxo/)
- HQ vehicle_class_id: 17
- Modelos:
  - [Ford Expedition](./suv-full-size-luxo/ford-expedition/)
  - [Chevrolet Suburban](./suv-full-size-luxo/chevrolet-suburban/)
  - [Dodge Durango](./suv-full-size-luxo/dodge-durango/)

### Conversivel (Mustang/Camaro)
- Pasta: [conversivel/](./conversivel/)
- HQ vehicle_class_id: 10
- Modelos:
  - [Mustang Conversivel](./conversivel/mustang-conversivel/)
  - [Camaro Conversivel](./conversivel/camaro-conversivel/)

### SUV Familia 6 Lugares
- Pasta: [suv-familia-6-lugares/](./suv-familia-6-lugares/)
- HQ vehicle_class_id: (nao mapeado)
- Modelos:
  - [Atlas](./suv-familia-6-lugares/atlas/)
  - [Traverse](./suv-familia-6-lugares/traverse/)
  - [Expedition](./suv-familia-6-lugares/expedition/)
  - [Tiguan](./suv-familia-6-lugares/tiguan/)
  - [Dodge Durango](./suv-familia-6-lugares/dodge-durango/)

### Truck (Camionete)
- Pasta: [truck/](./truck/)
- HQ vehicle_class_id: (nao mapeado)
- Modelos:
  - [Dodge Ram 1500](./truck/dodge-ram-1500/)

### Eletricos
- Pasta: [eletricos/](./eletricos/)
- HQ vehicle_class_id: (nao mapeado)
- Modelos:
  - [Tesla Model 3](./eletricos/tesla-model-3/)
  - [Cybertruck](./eletricos/cybertruck/)

## Como adicionar fotos

### 1) Direto pelo GitHub (mais simples)
1. Abra a pasta do modelo (ex: sedan-mid-size/toyota-corolla/)
2. Add file > Upload files - arrasta as fotos
3. Commit
4. Edita manifest.json incluindo o caminho

### 2) Via Telegram (a implementar)
Envia foto pro bot com /foto add slug/modelo - bot faz o commit auto.

## Convencao
- Nome: 01.jpg 02.jpg 03.jpg (ordem de preferencia)
- Bot pega aleatorio entre as 5 primeiras
- Max 5MB por foto
- Recomendado 1280x720 ou 1920x1080 JPG ~800KB
- jpg, jpeg ou png