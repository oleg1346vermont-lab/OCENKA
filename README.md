# mb_calculator — Transport System Efficiency Calculator

## English

A desktop application for the comparative evaluation of transport systems using the **M_b efficiency index**. Developed as part of a scientific study on transport infrastructure assessment for the Republic of Sakha (Yakutia).

**Five transport modes are covered:** road (trucks), river, railway, aviation, and airships.

**How it works:**

The application computes the M_b index for each transport mode:

```
M_b = (Pr × Re) / (L × R × I)
```

where:
- `Pr` — throughput productivity (load capacity × speed × distance × 24h / working hours)
- `Re` — annual revenue after tax
- `I` — total investment (fleet + infrastructure × efficiency rate + operating costs)
- `L` — constraint factor (path × personnel × infrastructure, each scored 1–3)
- `R` — risk factor (sum of technical, natural, human, and economic risks + 1)

**Application tabs:**
- **Summary** — ranked comparison of all five transport modes by M_b with a bar chart
- **Data** — editable parameter table; all baseline values can be modified, results recalculate instantly
- **Monte Carlo** — stochastic simulation (configurable iterations) producing distribution histograms and probability-of-dominance matrix
- **Sensitivity** — one-at-a-time sensitivity curves showing how M_b responds to ±20% variation in each parameter

**Running the app:**
- With Python: run `run.bat` — it sets up a virtual environment automatically on first launch
- Without Python: run `dist/mb_calculator.exe` — fully standalone, no installation required

**Best used for:** interactive exploration of transport efficiency scenarios, presentation of research results, and educational demonstration of multi-criteria transport assessment methodology.

**Requirements (for source run):** Python 3.8+, matplotlib, openpyxl. For the EXE — nothing.

---

## Русский

Десктопное приложение для сравнительной оценки транспортных систем по **показателю эффективности M_b**. Разработано в рамках научного исследования по оценке транспортной инфраструктуры Республики Саха (Якутия).

**Охватываемые виды транспорта:** автомобильный, речной, железнодорожный, авиационный, дирижабли.

**Принцип работы:**

Приложение вычисляет показатель M_b для каждого вида транспорта:

```
M_b = (Pr × Re) / (L × R × I)
```

где:
- `Pr` — производительность (грузоподъёмность × скорость × расстояние × 24 / рабочие часы)
- `Re` — годовая выручка после налогообложения
- `I` — суммарные инвестиции (парк + инфраструктура × норматив + эксплуатационные расходы)
- `L` — фактор ограничений (путь × персонал × инфраструктура, каждый 1–3)
- `R` — фактор рисков (сумма технических, природных, человеческих и экономических рисков + 1)

**Вкладки приложения:**
- **Сводка** — ранжированное сравнение всех пяти видов транспорта по M_b с гистограммой
- **Данные** — редактируемая таблица параметров; все базовые значения можно изменить, результаты пересчитываются мгновенно
- **Монте-Карло** — стохастическая симуляция (настраиваемое число итераций) с гистограммами распределения и матрицей вероятностей превосходства
- **Чувствительность** — однофакторные кривые, показывающие реакцию M_b на изменение каждого параметра в диапазоне ±20%

**Запуск:**
- С Python: запустить `run.bat` — при первом запуске автоматически создаётся виртуальная среда
- Без Python: запустить `dist/mb_calculator.exe` — полностью автономный, установка не нужна

**Область применения:** интерактивный анализ сценариев эффективности транспорта, презентация результатов исследований, учебная демонстрация методологии многокритериальной оценки транспортных систем.

**Зависимости (для запуска из исходников):** Python 3.8+, matplotlib, openpyxl. Для EXE — ничего не нужно.

---

## Монгол

**M_b үр ашгийн үзүүлэлт**-ээр тээврийн системийг харьцуулан үнэлэх ширээний програм. Саха (Якут) Бүгд Найрамдах Улсын тээврийн дэд бүтцийн үнэлгээний шинжлэх ухааны судалгааны хүрээнд боловсруулсан.

**Хамрах тээврийн төрлүүд:** авто, голын, төмөр зам, нисэх онгоц, дирижабль.

**Ажиллах зарчим:**

Програм нь тус бүр тээврийн хэрэгслэлд M_b үзүүлэлтийг тооцдог:

```
M_b = (Pr × Re) / (L × R × I)
```

Энд:
- `Pr` — бүтээмж (ачааны даац × хурд × зай × 24 / ажлын цаг)
- `Re` — татварын дараах жилийн орлого
- `I` — нийт хөрөнгө оруулалт (парк + дэд бүтэц × норматив + үйлдлийн зардал)
- `L` — хязгаарлалтын хүчин зүйл (зам × ажилтан × дэд бүтэц, 1–3 оноо)
- `R` — эрсдэлийн хүчин зүйл (техникийн, байгалийн, хүний, эдийн засгийн эрсдэлийн нийлбэр + 1)

**Програмын таб:**
- **Сводка** — таван тээврийн хэрэгслэлийг M_b-ээр жагсаан харьцуулах, баганан диаграм
- **Данные** — засварлах боломжтой параметрийн хүснэгт; суурь утгуудыг өөрчлөхөд үр дүн шууд дахин тооцоологдоно
- **Монте-Карло** — тохируулах боломжтой давталттай стохастик симуляци, тархалтын гистограм болон давуу байдлын магадлалын матриц
- **Чувствительность** — тус бүр параметрийн ±20% өөрчлөлтөд M_b хэрхэн хариу үйлдэл үзүүлэхийг харуулах нэг хүчин зүйлийн муруй

**Ажиллуулах:**
- Python-той: `run.bat` ажиллуул — анхны удаа автоматаар виртуал орчин үүснэ
- Python-гүй: `dist/mb_calculator.exe` ажиллуул — суулгалт огт шаардлагагүй

**Хэрэглэх хамгийн тохиромжтой газар:** тээврийн үр ашгийн хувилбаруудыг интерактив судлах, судалгааны үр дүнг танилцуулах, олон шалгуурт тээврийн үнэлгээний арга зүйг сургалтаар үзүүлэх.

**Шаардлага (эх кодоос ажиллуулахад):** Python 3.8+, matplotlib, openpyxl. EXE-д — юу ч шаардлагагүй.
