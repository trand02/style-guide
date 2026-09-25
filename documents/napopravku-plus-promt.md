# НаПоправку Плюс — бренд-контекст для ИИ-инструментов

Вставьте этот файл (или весь каталог) в контекст ChatGPT / Claude / Cursor, когда делаете что-либо
в фирменном стиле: презентацию, документ, лендинг, баннер, пост.

## Как пользоваться
1. Приложите этот файл + `README.md` (полный гайд: тон голоса, визуальные основы, иконография).
2. Приложите `tokens/*.css` — это единственный источник цветов, шрифтов, отступов и радиусов.
3. Просите результат в HTML: так он сразу совпадёт с токенами и его можно распечатать в PDF.

## Правила, которые нельзя нарушать
- Основные цвета — оранжевый `#FFB401` и голубой `#00B9D2`. Фиолетовый `#373660` — тёмная база
  для фонов и текста. Зелёный, красный и прочие — только как семантические статусы, не как акцент.
- Шрифт один: Montserrat (400/500/600/700). Заголовки — 600/700, текст — 400/500.
- Логотип: знак и логотип берутся из файлов, никогда не перерисовываются. На сложном фоне —
  белая плашка-подложка. Минимальный отступ вокруг знака — высота «кружка» знака.
- Никаких эмодзи, никаких сиренево-фиолетовых градиентов, никаких карточек с цветной полоской слева.
- Градиенты — только на обложках и разделителях: `linear-gradient` в оранжево-голубой или
  тёмно-фиолетовой гамме, углы 118–160°.
- Радиусы: 14px (мелкое), 20px (карточки), 28px (крупные плашки), 999px (чипы и кнопки-пилюли).
- Тон голоса: «вы», без канцелярита и медицинских страшилок, короткие утверждения, факт + польза.

## Токены (копия)
```css
/* ===== tokens/colors.css ===== */
:root{
/* brand — violet (primary) */
--violet-900:#8037FC;
--violet-600:#B387FD;
--violet-200:#E6D7FE;
--violet-100:#F2EBFF;
/* brand — orange */
--orange-900:#FFB401;
--orange-600:#FFD267;
--orange-200:#FEF0CB;
--orange-100:#FFF8E6;
/* brand — teal (secondary accent, "Blue" in guide) */
--teal-900:#00B9D2;
--teal-200:#CCF1F6;
--teal-100:#E6F8FB;
/* neutral — navy (used for dark surfaces + text) */
--navy-900:#373660;
--navy-800:#4B4A70;
--navy-600:#5E5E80;
--navy-400:#8686A0;
--navy-200:#B0AFBF;
--navy-100:#D7D7DF;
--white:#FFFFFF;
--black:#000000;
/* semantic */
--green-900:#23D376;
--green-200:#D3F5E4;
--green-100:#E9FAF0;
--red-900:#FF4956;
--red-200:#FFDBDD;
--red-100:#FFEDED;
/* raw text greys seen across the file */
--gray-text:#272728;
--gray-text-dark:#191B23;
--gray-text-muted:#7A7A7F;
/* semantic aliases */
--color-primary:var(--violet-900);
--color-accent:var(--orange-900);
--color-info:var(--teal-900);
--color-success:var(--green-900);
--color-error:var(--red-900);
--color-warning:var(--orange-900);
--text-heading:var(--navy-900);
--text-body:var(--gray-text);
--text-muted:var(--navy-400);
--text-inverse:var(--white);
--surface-page:var(--white);
--surface-card:var(--white);
--surface-brand:var(--violet-900);
--surface-brand-tint:var(--violet-100);
--border-default:var(--navy-100);
}


/* ===== tokens/typography.css ===== */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap');
:root{
--font-sans:'Montserrat',-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
--text-display:700 120px/1 var(--font-sans);
--text-h1:700 60px/1.1 var(--font-sans);
--text-h2:700 40px/1.2 var(--font-sans);
--text-h3:600 32px/1.4 var(--font-sans);
--text-h4:700 24px/1.3 var(--font-sans);
--text-label:400 40px/1.2 var(--font-sans);
--text-body-lg:400 24px/1.6 var(--font-sans);
--text-body:400 20px/1.6 var(--font-sans);
--text-body-sm:500 16px/1.6 var(--font-sans);
--text-caption:400 14px/1.5 var(--font-sans);
--tracking-tight:-0.02em;
--tracking-wide:0.02em;
}


/* ===== tokens/spacing.css ===== */
:root{
--space-1:4px;
--space-2:8px;
--space-3:10px;
--space-4:16px;
--space-5:20px;
--space-6:24px;
--space-7:27px;
--space-8:30px;
--space-9:40px;
--space-10:52px;
--space-11:60px;
--space-12:90px;
--space-13:100px;
}


/* ===== tokens/effects.css ===== */
:root{
--radius-sm:8px;
--radius-md:20px;
--radius-lg:38.67px;
--radius-xl:40px;
--radius-pill:999px;
--shadow-card:0 8px 21px rgba(31,70,76,0.16);
--shadow-ring:0 0 0 1.933px var(--border-default);
--shadow-soft:0 4px 12px rgba(0,0,0,0.1);
}

```
