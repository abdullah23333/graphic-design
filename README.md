<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>إنفوجرافيك التصميم الجرافيكي: رؤية أكاديمية</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Cairo', sans-serif;
            background-color: #001219;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 450px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .flowchart-step {
            transition: all 0.3s ease-in-out;
        }
        .flowchart-step:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(148, 210, 189, 0.2), 0 4px 6px -2px rgba(148, 210, 189, 0.1);
        }
        .flowchart-arrow {
            color: #94D2BD;
        }
    </style>
</head>
<body class="text-gray-200">

    <div class="container mx-auto px-4 sm:px-6 lg:px-8 py-12">

        <header class="text-center mb-16">
            <h1 class="text-4xl md:text-6xl font-black text-white mb-4"
            >التصميم الجرافيكي: رؤية أكاديمية</h1>
            <p class="text-lg md:text-xl text-[#94D2BD] max-w-3xl mx-auto">استكشاف تفاعلي للأسس والمجالات والعمليات التي تشكل عالم التواصل البصري الحديث.</p>
        </header>

        <main class="space-y-16">

            <section class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
                <div class="bg-[#003d4a] rounded-xl shadow-lg p-6 md:p-8">
                    <h2 class="text-3xl font-bold text-white mb-4">اللبنات الأساسية</h2>
                    <p class="mb-6 text-gray-300">كل تصميم عظيم يرتكز على مجموعة من العناصر والمبادئ الأساسية. العناصر هي الأدوات التي تستخدمها، والمبادئ هي القواعد التي توجه كيفية استخدامها بفعالية.</p>
                    <div class="grid grid-cols-2 gap-6">
                        <div>
                            <h3 class="text-xl font-bold text-[#94D2BD] mb-3">عناصر التصميم</h3>
                            <ul class="space-y-2">
                                <li class="flex items-center"><span class="text-[#EE9B00] ml-3 text-xl">📏</span> الخط</li>
                                <li class="flex items-center"><span class="text-[#EE9B00] ml-3 text-xl">🖼️</span> الشكل</li>
                                <li class="flex items-center"><span class="text-[#EE9B00] ml-3 text-xl">🎨</span> اللون</li>
                                <li class="flex items-center"><span class="text-[#EE9B00] ml-3 text-xl">📝</span> الطباعة</li>
                                <li class="flex items-center"><span class="text-[#EE9B00] ml-3 text-xl">🧱</span> الملمس</li>
                                <li class="flex items-center"><span class="text-[#EE9B00] ml-3 text-xl">🌌</span> المساحة</li>
                            </ul>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-[#94D2BD] mb-3">مبادئ التصميم</h3>
                            <ul class="space-y-2">
                                <li class="flex items-center"><span class="text-[#CA6702] ml-3 text-xl">⚖️</span> التوازن</li>
                                <li class="flex items-center"><span class="text-[#CA6702] ml-3 text-xl">🌗</span> التباين</li>
                                <li class="flex items-center"><span class="text-[#CA6702] ml-3 text-xl">ιε</span> التسلسل الهرمي</li>
                                <li class="flex items-center"><span class="text-[#CA6702] ml-3 text-xl">📐</span> المحاذاة</li>
                                <li class="flex items-center"><span class="text-[#CA6702] ml-3 text-xl">🧩</span> التقارب</li>
                                <li class="flex items-center"><span class="text-[#CA6702] ml-3 text-xl">🔄</span> التكرار</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="bg-[#003d4a] rounded-xl shadow-lg p-6 md:p-8">
                    <h2 class="text-3xl font-bold text-white mb-2">توزيع مجالات التصميم</h2>
                     <p class="mb-4 text-gray-300">يتفرع التصميم الجرافيكي إلى تخصصات متنوعة، لكل منها طلب وتركيز مختلف في سوق العمل. يوضح الرسم البياني التالي توزيعًا تقديريًا لهذه المجالات.</p>
                    <div class="chart-container">
                        <canvas id="fieldsChart"></canvas>
                    </div>
                </div>
            </section>

            <section class="bg-[#003d4a] rounded-xl shadow-lg p-6 md:p-8">
                <div class="text-center">
                    <h2 class="text-3xl font-bold text-white mb-2">عملية التصميم الأكاديمية</h2>
                    <p class="mb-8 text-gray-300 max-w-3xl mx-auto">يمر كل مشروع تصميم ناجح بسلسلة من الخطوات المنهجية التي تضمن تحقيق الأهداف بفعالية، من الفهم الأولي إلى التسليم النهائي.</p>
                </div>
                <div class="flex flex-col md:flex-row items-center justify-center space-y-4 md:space-y-0 md:space-x-4 rtl:md:space-x-reverse">
                    <div class="flowchart-step bg-[#0A9396] text-white p-4 rounded-lg text-center w-full md:w-48">
                        <div class="text-3xl font-black">1</div>
                        <div class="font-bold mt-1">الفكرة والبحث</div>
                    </div>
                    <div class="text-4xl flowchart-arrow hidden md:block">&rarr;</div>
                     <div class="text-4xl flowchart-arrow block md:hidden">&darr;</div>
                    <div class="flowchart-step bg-[#94D2BD] text-black p-4 rounded-lg text-center w-full md:w-48">
                        <div class="text-3xl font-black">2</div>
                        <div class="font-bold mt-1">التخطيط والرسم</div>
                    </div>
                    <div class="text-4xl flowchart-arrow hidden md:block">&rarr;</div>
                     <div class="text-4xl flowchart-arrow block md:hidden">&darr;</div>
                    <div class="flowchart-step bg-[#E9D8A6] text-black p-4 rounded-lg text-center w-full md:w-48">
                        <div class="text-3xl font-black">3</div>
                        <div class="font-bold mt-1">التنفيذ الرقمي</div>
                    </div>
                     <div class="text-4xl flowchart-arrow hidden md:block">&rarr;</div>
                     <div class="text-4xl flowchart-arrow block md:hidden">&darr;</div>
                    <div class="flowchart-step bg-[#EE9B00] text-black p-4 rounded-lg text-center w-full md:w-48">
                        <div class="text-3xl font-black">4</div>
                        <div class="font-bold mt-1">المراجعة والتعديل</div>
                    </div>
                     <div class="text-4xl flowchart-arrow hidden md:block">&rarr;</div>
                     <div class="text-4xl flowchart-arrow block md:hidden">&darr;</div>
                    <div class="flowchart-step bg-[#CA6702] text-white p-4 rounded-lg text-center w-full md:w-48">
                        <div class="text-3xl font-black">5</div>
                        <div class="font-bold mt-1">المنتج النهائي</div>
                    </div>
                </div>
            </section>
            
            <section class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
                 <div class="bg-[#003d4a] rounded-xl shadow-lg p-6 md:p-8">
                    <h2 class="text-3xl font-bold text-white mb-2">شعبية برامج التصميم</h2>
                     <p class="mb-4 text-gray-300">تتنوع الأدوات التي يستخدمها المصممون. يوضح هذا الرسم مقارنة لشعبية أشهر برامج التصميم بناءً على استطلاعات الصناعة وتوجهات السوق الحالية.</p>
                    <div class="chart-container h-96">
                        <canvas id="toolsChart"></canvas>
                    </div>
                </div>
                <div class="bg-[#003d4a] rounded-xl shadow-lg p-6 md:p-8">
                    <h2 class="text-3xl font-bold text-white mb-4">نصائح ذهبية للتصميم</h2>
                    <p class="mb-6 text-gray-300">لتحويل تصميم جيد إلى تصميم استثنائي، إليك بعض النصائح العملية المستوحاة من الخبراء، والتي يمكن تطبيقها مباشرة في برامج مثل Adobe Illustrator.</p>
                    <ul class="space-y-4">
                        <li class="p-4 bg-[#0A9396] rounded-lg">
                            <h3 class="font-bold text-lg text-white">استخدم نظامًا شبكيًا (Grid)</h3>
                            <p class="text-gray-100">يمنحك أساسًا متينًا للمحاذاة ويضفي مظهرًا منظمًا واحترافيًا.</p>
                        </li>
                        <li class="p-4 bg-[#94D2BD] rounded-lg">
                            <h3 class="font-bold text-lg text-black">اختر ألوانك بحكمة</h3>
                            <p class="text-gray-800">اكتفِ بلونين أو ثلاثة ألوان رئيسية للحفاظ على التناسق البصري.</p>
                        </li>
                        <li class="p-4 bg-[#E9D8A6] rounded-lg">
                            <h3 class="font-bold text-lg text-black">بساطة الخطوط قوة</h3>
                            <p class="text-gray-800">استخدم خطًا واحدًا أو اثنين على الأكثر لضمان الوضوح وسهولة القراءة.</p>
                        </li>
                         <li class="p-4 bg-[#EE9B00] rounded-lg">
                            <h3 class="font-bold text-lg text-black">عناق المساحة البيضاء</h3>
                            <p class="text-gray-800">لا تخف من الفراغ، فهو يساعد على راحة العين وتركيزها على المهم.</p>
                        </li>
                    </ul>
                </div>
            </section>

        </main>

        <footer class="text-center mt-16 pt-8 border-t border-gray-700">
            <p class="text-gray-400">&copy; 2025 من إعداد: المدرب عبدالله الوادي</p>
        </footer>

    </div>

    <script>
        const tooltipTitleCallback = (tooltipItems) => {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
                return label.join(' ');
            }
            return label;
        };
        
        const wrapLabel = (label) => {
            const maxLength = 16;
            if (label.length <= maxLength) {
                return label;
            }
            const words = label.split(' ');
            const lines = [];
            let currentLine = '';
            words.forEach(word => {
                if ((currentLine + word).length > maxLength) {
                    lines.push(currentLine.trim());
                    currentLine = '';
                }
                currentLine += word + ' ';
            });
            lines.push(currentLine.trim());
            return lines;
        };

        const fieldsCtx = document.getElementById('fieldsChart').getContext('2d');
        const fieldsChart = new Chart(fieldsCtx, {
            type: 'doughnut',
            data: {
                labels: ['التصميم الرقمي والويب', 'تصميم الهوية البصرية', 'تصميم المطبوعات', 'التعبئة والتغليف', 'الرسوم التوضيحية'],
                datasets: [{
                    label: 'توزيع مجالات التصميم',
                    data: [40, 30, 15, 10, 5],
                    backgroundColor: ['#0A9396', '#94D2BD', '#E9D8A6', '#EE9B00', '#CA6702'],
                    borderColor: '#003d4a',
                    borderWidth: 4,
                    hoverOffset: 10
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            color: '#E9D8A6',
                            font: {
                                size: 14,
                                family: "'Cairo', sans-serif"
                            }
                        }
                    },
                    tooltip: {
                        callbacks: {
                            title: tooltipTitleCallback
                        }
                    }
                },
                cutout: '60%'
            }
        });

        const toolsCtx = document.getElementById('toolsChart').getContext('2d');
        const originalToolsLabels = ['Adobe Illustrator', 'Adobe Photoshop', 'Figma', 'Canva', 'Adobe InDesign', 'CorelDRAW'];
        const processedToolsLabels = originalToolsLabels.map(wrapLabel);
        
        const toolsChart = new Chart(toolsCtx, {
            type: 'bar',
            data: {
                labels: processedToolsLabels,
                datasets: [{
                    label: 'نسبة الاستخدام بين المحترفين',
                    data: [85, 78, 90, 65, 55, 30],
                    backgroundColor: ['#EE9B00', '#CA6702', '#AE2012', '#9B2226', '#0A9396', '#005F73'],
                    borderColor: '#003d4a',
                    borderWidth: 2,
                    borderRadius: 5
                }]
            },
            options: {
                indexAxis: 'y',
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    x: {
                        beginAtZero: true,
                        grid: {
                            color: 'rgba(148, 210, 189, 0.2)'
                        },
                        ticks: {
                            color: '#94D2BD',
                            font: {
                                family: "'Cairo', sans-serif"
                            }
                        }
                    },
                    y: {
                        grid: {
                            display: false
                        },
                        ticks: {
                            color: '#E9D8A6',
                            font: {
                                size: 14,
                                family: "'Cairo', sans-serif"
                            }
                        }
                    }
                },
                plugins: {
                    legend: {
                        display: false
                    },
                    tooltip: {
                        callbacks: {
                            title: tooltipTitleCallback
                        }
                    }
                }
            }
        });
    </script>
</body>
</html>
