# NeoFamily Blog — Мультиагентный пайплайн

## Ссылки проекта
- **Figma (рабочий файл):** https://www.figma.com/design/2V3f7LR4hyenHFdSdLGArs/WP-testing-Claude-Code-for-NeoFamily
- **Figma (UI Kit):** https://www.figma.com/design/mqEAVDMnFPpj63fjZQhJP0/neoFamily_P.2?node-id=2-16735
- **Конкурент (Умскул):** https://umschool.net/journal/
- **Сайт компании:** https://neofamily.ru/
- **ТЗ на дизайн:** https://docs.google.com/document/d/1-z-NtHXOPO9cvGpetcrNzvelp6WxFWNP6HnEFihfzrs/
- **ТЗ на WordPress:** https://docs.google.com/document/d/1hCsmRCOAE8-bw-P-s5ZYJdnVKqVRHWQotdBwm9GrMnY/

## Агенты
| # | Агент | Папка | Роль |
|---|-------|-------|------|
| 1 | Project Manager | `project_manager/` | Контроль соответствия ТЗ |
| 2 | UX/UI Designer | `designer/` | Дизайн и прототипирование в Figma |
| 3 | Маркетолог | `marketer/` | Рекомендации по подаче и конверсии |
| 4 | Tech Lead | `tech_lead/` | Техническая реализуемость на WordPress |
| 5 | Fact-checker | `fact_checker/` | Проверка фактов о компании |
| 6 | SEO-специалист | `seo_specialist/` | SEO-оптимизация структуры и макетов |

## Этапы

### Этап 1: Сбор и анализ требований ✅ DONE
- **Fact-checker** → `company_profile.md` ✅
- **Tech Lead** → `wp_requirements.md` ✅
- **Маркетолог** → `competitor_analysis.md` + `recommendations.md` ✅
- **SEO-специалист** → `seo_recommendations.md` ✅
- **Designer** → `tokens.md` ✅
- **PM** → `shared/requirements/brief.md` ✅

### Этап 2: Концепция дизайна ✅ APPROVED
- **Designer** → `concept.md` v1.1 ✅ (все замечания учтены)
- **Designer** → `figma_spec.md` ✅ (3/6 страниц детально, остальные в concept)
- **Маркетолог** → `review.md` ✅ (10 замечаний P1, 0 блокеров)
- **Tech Lead** → `tech_review.md` ✅ (8 замечаний, 0 блокеров)
- **PM** → `stage2_review.md` ✅ APPROVED (6/6 страниц, 8/8 компонентов, 12/12 блоков)

### Этап 3: Прототип в Figma ← ТЕКУЩИЙ
- **Designer** → отрисовка макетов в Figma по figma_spec.md
- **PM** → сверка с ТЗ
- **Tech Lead** → финальная техническая проверка

### Этап 4: Разработка WordPress
- Вёрстка темы на основе утверждённых макетов
- Настройка Yoast SEO, JSON-LD, шорткоды
- Tech Lead контролирует

## Статус: ЭТАП 3 — IN PROGRESS
