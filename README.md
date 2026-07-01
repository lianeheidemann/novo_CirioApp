# CírioApp

Aplicativo mobile informativo sobre o Círio de Nazaré — Belém do Pará. A maior procissão católica do Brasil, na palma da sua mão.

![Flutter](https://img.shields.io/badge/Flutter-3.16+-02569B?style=flat-square)
![Dart](https://img.shields.io/badge/Dart-3.0+-0175C2?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Android-brightgreen?style=flat-square)

---

## Visão Geral

CírioApp é um aplicativo mobile desenvolvido em Flutter que centraliza informações sobre o Círio de Nazaré, incluindo programação de eventos, mapa interativo, notícias e sistema de favoritos.

---

## Funcionalidades

- Eventos — Calendário completo com datas, horários e locais
- Mapa Interativo — OpenStreetMap com pontos de interesse categorizados
- Notícias — Feed atualizado com conteúdo sobre o Círio
- Favoritos — Sistema sincronizado para eventos, locais e notícias
- Persistência Local — Dados salvos automaticamente

---

## Tecnologias

| Tecnologia | Versão |
|---|---|
| Flutter | 3.16+ |
| Dart | 3.0+ |
| Provider | ^6.1.2 |
| flutter_map | ^6.1.0 |
| shared_preferences | ^2.2.3 |
| cached_network_image | ^3.3.1 |

---

## Arquitetura

Estrutura em camadas com separação de responsabilidades:

```
lib/
├── core/              # Constantes e tema
├── data/              # Modelos, serviços e repositórios
├── features/          # Funcionalidades autocontidas
└── shared/            # Componentes reutilizáveis
```

Gerenciamento de estado: Provider com ChangeNotifier

---

## Como Executar

Pré-requisitos:
- Flutter SDK `>=3.0.0 <4.0.0`
- Android SDK 21+
- Conexão com internet

Passos:

```bash
git clone https://github.com/lianeheidemann/novo_CirioApp.git
cd novo_CirioApp
flutter pub get
flutter run
```

Build release:
```bash
flutter build apk --release
```

---

## Estrutura de Arquivos

```
lib/
├── main.dart                      (41 linhas)
├── app.dart                       (21 linhas)
├── core/
│   ├── theme/app_theme.dart       (70 linhas)
│   └── constants/                 (16 linhas)
├── data/
│   ├── models/                    (123 linhas)
│   ├── services/                  (339 linhas)
│   ├── repositories/              (27 linhas)
│   └── local/                     (43 linhas)
├─�� features/
│   ├── home/                      (240 linhas)
│   ├── events/                    (349 linhas)
│   ├── places/                    (413 linhas)
│   ├── map/                       (198 linhas)
│   ├── news/                      (286 linhas)
│   └── favorites/                 (269 linhas)
└── shared/widgets/                (94 linhas)
```

---

## Contribuindo

1. Fork o projeto
2. Crie uma branch (`git checkout -b feature/MinhaFeature`)
3. Commit as mudanças (`git commit -m 'feat: descrição'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

---

<img width="100%" src="https://github.com/user-attachments/assets/f29362d6-449f-4676-8de8-f7d4f0e3139a" alt="CírioApp Screenshots" />
