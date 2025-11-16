# المختار التركيبي / Syntactic Selector

<div dir="rtl">

أداة متقدمة لتحليل التراكيب اللغوية العربية باستخدام المقاييس الإحصائية (PMI, T-Score, Log-Likelihood) مع واجهة تفاعلية متقدمة.

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

</div>

## المميزات

- **تحليل إحصائي متقدم**: حساب PMI، T-Score، Log-Likelihood للتراكيب
- **واجهة تفاعلية متقدمة**: خريطة حرارية، رسوم ثلاثية الأبعاد، مخطط Chord
- **حفظ السياقات النصية**: عرض أمثلة سياقية لكل تركيب
- **تصدير متعدد الصيغ**: Excel و JSON
- **إحصائيات مفصلة**: تحليل شامل للملفات والتراكيب
- **فلترة ديناميكية**: تصفية وترتيب النتائج حسب معايير متعددة

## المتطلبات

- Python 3.7 أو أحدث
- pandas
- openpyxl

## التثبيت

1. استنسخ المستودع:
```bash
git clone https://github.com/ayzem88/syntactic-selector.git
cd syntactic-selector
```

2. ثبت المتطلبات:
```bash
pip install -r requirements.txt
```

3. **ملاحظة مهمة**: البرنامج يحتاج ملفات نصية في مجلد `المدونة/` للتحليل. هذه الملفات كبيرة ولم يتم رفعها على GitHub.

   **الحلول**:
   - أضف ملفات `.txt` الخاصة بك في مجلد `المدونة/`
   - البرنامج سيعمل مع أي ملفات نصية تضيفها
   - ملف `stop_words.txt` موجود ومرفوع

## الاستخدام

### الخطوة 1: تشغيل السكربت

```bash
python "0.2 المختار التركيبي.py"
```

أو النسخة المحسنة:
```bash
python "كشكول/المختار_التركيبي_المحسن_مختصر.py"
```

### الخطوة 2: فتح الواجهة التفاعلية

1. افتح ملف `02. المختار التركيبي التفاعلي.html` في المتصفح
2. أو استخدم خادم محلي:
```bash
python -m http.server 8000
# ثم افتح http://localhost:8000/02.%20المختار%20التركيبي%20التفاعلي.html
```

### الخطوة 3: تحميل البيانات

- اختر ملف `البيانات_التفاعلية.json` المُنشأ
- أو استخدم "تحميل بيانات تجريبية" للعرض

## الملفات

- `0.2 المختار التركيبي.py`: السكربت الرئيسي
- `02. المختار التركيبي التفاعلي.html`: الواجهة التفاعلية
- `البيانات_التفاعلية.json`: ملف البيانات المُصدّر
- `المركبات_المحسنة.xlsx`: ملف Excel مع النتائج
- `stop_words.txt`: ملف كلمات الإيقاف
- `المدونة/`: مجلد ملفات النصوص للتحليل

## الرسوم البيانية المتاحة

### 1. الخريطة الحرارية
تُظهر توزيع التراكيب عبر الملفات مع تمييز الألوان حسب الكثافة.

### 2. الرسم ثلاثي الأبعاد
عرض المقاييس الإحصائية (PMI, T-Score, Log-Likelihood) في فضاء ثلاثي الأبعاد.

### 3. مخطط Chord
يربط التراكيب المتشابهة مع تمييز قوة الارتباط.

### 4. شجرة القرار
تُظهر منطق الترجيح وتقسيم المعايير.

### 5. جدول تفاعلي
جميع البيانات مع إمكانية الفلترة والترتيب.

## الميزات التفاعلية

- **الفلترة**: تصفية حسب نوع الترجيح
- **الترتيب**: حسب PMI، التكرار، الانتشار، التنوع السياقي
- **عرض السياقات**: انقر على "عرض السياقات" لرؤية النماذج النصية
- **الإحصائيات**: تحديث فوري مع الفلترة

## الإحصائيات

- **445,208** تركيبة تم تحليلها
- **113,095** كلمة مفردة
- **18** ملف نصي
- **5** سياقات محفوظة لكل تركيب

## الاختبار

```bash
# تثبيت متطلبات التطوير
pip install -r requirements-dev.txt

# تشغيل الاختبارات
python -m pytest tests/
```

## المساهمة

نرحب بمساهماتكم! راجع [دليل المساهمة](CONTRIBUTING.md) للتفاصيل.

## الترخيص

هذا المشروع مرخص تحت [MIT License](LICENSE) - راجع ملف LICENSE للتفاصيل.

## المطور

تم تطوير هذا المشروع بواسطة **أيمن الطيّب بن نجي** ([ayzem88](https://github.com/ayzem88))

## التواصل

للاستفسارات أو المساهمة، يمكنك التواصل معي عبر:
- البريد الإلكتروني: [aymen.nji@gmail.com](mailto:aymen.nji@gmail.com)

## التطوير المستقبلي

- [ ] إضافة مقارنة مع corpus مرجعي
- [ ] شريط زمني تفاعلي
- [ ] تصدير التقارير بصيغ مختلفة
- [ ] دعم لغات إضافية
- [ ] واجهة سطر الأوامر (CLI)

## الصور

![صورة 1](img-01.png)
![صورة 2](img-02.png)
![صورة 3](img-03.png)

---

# [English]

<div dir="ltr">

## Syntactic Selector

An advanced tool for analyzing Arabic linguistic structures using statistical measures (PMI, T-Score, Log-Likelihood) with an advanced interactive interface.

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Features

- **Advanced Statistical Analysis**: Calculate PMI, T-Score, Log-Likelihood for structures
- **Advanced Interactive Interface**: Heatmap, 3D plots, Chord diagram
- **Context Preservation**: Display contextual examples for each structure
- **Multiple Export Formats**: Excel and JSON
- **Detailed Statistics**: Comprehensive analysis of files and structures
- **Dynamic Filtering**: Filter and sort results by multiple criteria

## Requirements

- Python 3.7 or later
- pandas
- openpyxl

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ayzem88/syntactic-selector.git
cd syntactic-selector
```

2. Install requirements:
```bash
pip install -r requirements.txt
```

3. **Important Note**: The program needs text files in the `المدونة/` folder for analysis. These files are large and were not uploaded to GitHub.

   **Solutions**:
   - Add your own `.txt` files in the `المدونة/` folder
   - The program will work with any text files you add
   - The `stop_words.txt` file is included and uploaded

## Usage

### Step 1: Run the Script

```bash
python "0.2 المختار التركيبي.py"
```

Or the enhanced version:
```bash
python "كشكول/المختار_التركيبي_المحسن_مختصر.py"
```

### Step 2: Open the Interactive Interface

1. Open the `02. المختار التركيبي التفاعلي.html` file in your browser
2. Or use a local server:
```bash
python -m http.server 8000
# Then open http://localhost:8000/02.%20المختار%20التركيبي%20التفاعلي.html
```

### Step 3: Load Data

- Choose the generated `البيانات_التفاعلية.json` file
- Or use "Load sample data" for display

## Files

- `0.2 المختار التركيبي.py`: Main script
- `02. المختار التركيبي التفاعلي.html`: Interactive interface
- `البيانات_التفاعلية.json`: Exported data file
- `المركبات_المحسنة.xlsx`: Excel file with results
- `stop_words.txt`: Stop words file
- `المدونة/`: Folder for text files to analyze

## Available Charts

### 1. Heatmap
Shows the distribution of structures across files with color coding by density.

### 2. 3D Plot
Displays statistical measures (PMI, T-Score, Log-Likelihood) in 3D space.

### 3. Chord Diagram
Links similar structures with connection strength indication.

### 4. Decision Tree
Shows weighting logic and criteria division.

### 5. Interactive Table
All data with filtering and sorting capabilities.

## Interactive Features

- **Filtering**: Filter by weighting type
- **Sorting**: By PMI, frequency, spread, contextual diversity
- **Context Display**: Click "Show contexts" to see text examples
- **Statistics**: Real-time updates with filtering

## Statistics

- **445,208** structures analyzed
- **113,095** unique words
- **18** text files
- **5** contexts saved per structure

## Testing

```bash
# Install development requirements
pip install -r requirements-dev.txt

# Run tests
python -m pytest tests/
```

## Contributing

We welcome contributions! See [Contributing Guide](CONTRIBUTING.md) for details.

## License

This project is licensed under [MIT License](LICENSE) - see the LICENSE file for details.

## Developer

Developed by **Ayman Al-Tayyib Ben Naji** ([ayzem88](https://github.com/ayzem88))

## Contact

For inquiries or contributions, you can contact me via:
- Email: [aymen.nji@gmail.com](mailto:aymen.nji@gmail.com)

## Future Development

- [ ] Add comparison with reference corpus
- [ ] Interactive timeline
- [ ] Export reports in different formats
- [ ] Support for additional languages
- [ ] Command-line interface (CLI)

## Screenshots

![Screenshot 1](img-01.png)
![Screenshot 2](img-02.png)
![Screenshot 3](img-03.png)

</div>

