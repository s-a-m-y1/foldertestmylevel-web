Egypt Tourism
│
├── 🏠 Home
│
├── 🏛️ Destinations
│     ├── Pyramids
│     ├── Luxor
│     ├── Aswan
│     └── Red Sea
│
├── 📸 Gallery
│
├── 🔐 Login
│
├── 📝 Register
│
└── 📞 Contact

لكن مش هنعملهم مرة واحدة.

هنبني المشروع تدريجيًا.

1. Home Page

مثلاً:

┌──────────────────────────────────────────────┐
│ 🇪🇬 Egypt       Home  Places  Gallery Login │
├──────────────────────────────────────────────┤
│                                              │
│          DISCOVER EGYPT                      │
│                                              │
│      The land of history                     │
│                                              │
│        [ Explore Now ]                       │
│                                              │
└──────────────────────────────────────────────┘

هنا هتتعلم:

background-image
background-size
background-position
Flexbox
positioning
buttons
typography
hover
transitions
vh
2. Navigation Bar
┌──────────────────────────────────────────────┐
│ 🇪🇬 EGYPT     Home   Places   Gallery  Login │
└──────────────────────────────────────────────┘

هنا:

display: flex;
justify-content: space-between;
align-items: center;
gap: ...

وهتتعلم كمان:

position: sticky;
3. Destinations

نعمل Cards:

┌───────────┐  ┌───────────┐  ┌───────────┐
│  PYRAMID  │  │   LUXOR   │  │   ASWAN   │
│   IMAGE   │  │   IMAGE   │  │   IMAGE   │
│           │  │           │  │           │
│ Learn More│  │ Learn More│  │ Learn More│
└───────────┘  └───────────┘  └───────────┘

هنا تستخدم:

display: grid;

grid-template-columns:
repeat(3, 1fr);

gap: 20px;

وبالتالي تتعلم Grid فعليًا.

4. Responsive

على الكمبيوتر:

┌─────┐ ┌─────┐ ┌─────┐
│     │ │     │ │     │
└─────┘ └─────┘ └─────┘

على الموبايل:

┌─────────────┐
│             │
└─────────────┘

┌─────────────┐
│             │
└─────────────┘

┌─────────────┐
│             │
└─────────────┘

باستخدام:

@media (max-width: 768px) {

    .cards {
        grid-template-columns: 1fr;
    }

}

وهنا هتفهم Media Queries بجد.

5. Gallery

نعمل Gallery مختلفة شوية:

┌────────┬────────┬────────┐
│        │        │        │
│ Image  │ Image  │ Image  │
│        │        │        │
├────────┼────────┼────────┤
│        │        │        │
│ Image  │ Image  │ Image  │
│        │        │        │
└────────┴────────┴────────┘

هنا هنستخدم:

Grid
grid-template-columns
grid-template-rows
object-fit
gap
hover
transform
transition
6. Login Form

نعمل:

┌────────────────────────┐
│        Welcome Back    │
│                        │
│  Email                 │
│  ┌──────────────────┐  │
│  │                  │  │
│  └──────────────────┘  │
│                        │
│  Password              │
│  ┌──────────────────┐  │
│  │                  │  │
│  └──────────────────┘  │
│                        │
│       [ Login ]        │
│                        │
│   Create an account    │
└────────────────────────┘

هنا هتطبق:

Form
Input
Button
Flexbox
Box Model
:focus
:hover
transitions
positioning
7. Register Form

ودي اللي أنت تقصدها بـ:

الفورم تروح للفورم التانية

بالضبط.

مثلاً:

Login
  │
  │ Create Account
  ↓
Register

وفي Register:

┌────────────────────────┐
│      Create Account    │
│                        │
│ Full Name              │
│ Email                  │
│ Password               │
│ Confirm Password       │
│                        │
│    [ Register ]        │
│                        │
│ Already have account?  │
│        Login           │
└────────────────────────┘

والـ Login يرجع إلى Register والعكس.

في البداية نعمل التنقل بـ HTML:

<a href="register.html">
    Create Account
</a>

وبعدين لما تدخل JavaScript نبدأ نخلي الـ Forms تفاعلية.

8. Contact Form

وفي الآخر:

┌─────────────────────────────────┐
│          Contact Us             │
│                                 │
│ Name                            │
│ ┌─────────────────────────────┐ │
│ └─────────────────────────────┘ │
│                                 │
│ Email                           │
│ ┌─────────────────────────────┐ │
│ └─────────────────────────────┘ │
│                                 │
│ Message                         │
│ ┌─────────────────────────────┐ │
│ │                             │ │
│ │                             │ │
│ └─────────────────────────────┘ │
│                                 │
│          [ Send ]               │
└─────────────────────────────────┘

وهنا نتعلم:

textarea

وكمان:

resize
9. Footer
─────────────────────────────────────

        🇪🇬 Discover Egypt

     Home | Places | Gallery | Contact

           © 2026 Egypt

─────────────────────────────────────

وهنا نطبق Flexbox + Responsive.

والمميز في المشروع ده

إنه هيجمع تقريبًا كل اللي سألت عنه:

CSS Concept	هنستخدمه فين؟
Selectors	كل المشروع
Box Model	Forms / Cards
Margin	كل الـ layouts
Padding	Cards / Forms
Border	Inputs / Cards
Border-radius	Buttons / Cards
Colors	كل المشروع
Fonts	Typography
Flexbox	Navbar / Forms
Grid	Cards / Gallery
gap	Flex + Grid
Position	Hero / Navbar
absolute	Hero elements
sticky	Navbar
z-index	Hero/Navbar
background-image	Hero
object-fit	الصور
:hover	Buttons / Cards
:focus	Inputs
transition	Animations
transform	Cards
@media	Mobile
%	Responsive
rem	Fonts
vh	Hero
CSS Variables	Theme
والأهم: المشروع هيكون على مرحلتين
المرحلة الأولى — HTML + CSS
HTML
 ↓
CSS
 ↓
Responsive
 ↓
Forms
 ↓
Navigation

ممنوع JavaScript في المرحلة دي.

لأن هدفنا نشوف هل تقدر تبني الموقع بنفسك باستخدام HTML + CSS فقط.

المرحلة الثانية — JavaScript

بعد ما نخلص CSS:

JavaScript
     ↓
DOM
     ↓
Events
     ↓
Login validation
     ↓
Register validation
     ↓
Form handling
     ↓
Dark / Light mode
     ↓
LocalStorage
     ↓
API

وده هيكون انتقال ممتاز من CSS → JavaScript بدل ما تدخل JS من غير مشروع تطبق عليه.

وبما إنك بتتعلم خطوة بخطوة، أنا أنصحنا نبنيه من الصفر، جزء جزء، ومش أديك المشروع كامل مرة واحدة.