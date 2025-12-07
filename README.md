# website
<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Економічна безпека Італії</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #3B3030;
            background: #F9F8F6;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            background: #E7CCCC;
            color: #3B3030;
            padding: 30px 0;
            text-align: center;
            margin-bottom: 30px;
            border-radius: 8px;
        }

        header h1 {
            font-size: 2.2em;
            margin-bottom: 10px;
        }

        .nav {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .nav-btn {
            padding: 12px 28px;
            background: #E7CCCC;
            color: #3B3030;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background 0.3s;
            font-weight: 500;
        }

        .nav-btn:hover {
            background: #EDDFE0;
        }

        .nav-btn.active {
            background: #EDDFE0;
        }

        .page {
            display: none;
            background: white;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .page.active {
            display: block;
            animation: fadeIn 0.4s;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        h2 {
            color: #3B3030;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid #E7CCCC;
        }

        h3 {
            color: #3B3030;
            margin-top: 20px;
            margin-bottom: 10px;
        }

        .resume-section {
            background: #F9F8F6;
            padding: 20px;
            margin: 15px 0;
            border-radius: 5px;
            border-left: 4px solid #E7CCCC;
        }

        .resume-section p {
            margin: 8px 0;
        }

        .resume-section strong {
            color: #3B3030;
        }

        .analysis-text {
            background: #F9F8F6;
            padding: 25px;
            margin: 20px 0;
            border-radius: 5px;
            text-align: justify;
            line-height: 1.8;
        }

        .analysis-text p {
            margin-bottom: 15px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background: white;
            border: 2px solid #E7CCCC;
        }

        table thead {
            background: #E7CCCC;
            color: #3B3030;
        }

        table th {
            padding: 12px;
            text-align: left;
            border: 1px solid #E7CCCC;
            font-weight: 600;
        }

        table td {
            padding: 12px;
            text-align: left;
            border: 1px solid #EDDFE0;
        }

        table tbody tr:nth-child(even) {
            background: #F9F8F6;
        }

        table tbody tr:hover {
            background: #EDDFE0;
        }

        .chart-container {
            margin: 30px 0;
            padding: 20px;
            background: #F9F8F6;
            border-radius: 5px;
        }

        .chart-bar {
            display: flex;
            align-items: center;
            margin: 15px 0;
        }

        .chart-label {
            width: 200px;
            font-weight: 500;
            color: #3B3030;
        }

        .chart-bar-fill {
            height: 30px;
            background: linear-gradient(90deg, #E7CCCC 0%, #EDDFE0 100%);
            border-radius: 3px;
            display: flex;
            align-items: center;
            padding: 0 10px;
            color: #3B3030;
            font-weight: bold;
        }

        .indicator {
            display: inline-block;
            padding: 5px 15px;
            background: #E7CCCC;
            color: #3B3030;
            border-radius: 3px;
            margin: 5px 5px 5px 0;
            font-size: 0.95em;
        }

        ul {
            margin-left: 20px;
            margin-top: 10px;
        }

        li {
            margin: 10px 0;
        }

        .table-container {
            margin: 30px 0;
        }

        .table-title {
            background: #E7CCCC;
            color: #3B3030;
            padding: 12px;
            font-weight: bold;
            border-radius: 5px 5px 0 0;
            text-align: center;
            font-size: 1.1em;
        }

        .number-cell {
            width: 50px;
            text-align: center;
            font-weight: bold;
            background: #EDDFE0;
        }

        .name-cell {
            width: 30%;
            font-weight: 600;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Економічна безпека Італії</h1>
            <p>Аналітичне дослідження стану та перспектив</p>
        </header>

        <div class="nav">
            <button class="nav-btn active" onclick="showPage(1)">Резюме</button>
            <button class="nav-btn" onclick="showPage(2)">Економічна безпека країни</button>
            <button class="nav-btn" onclick="showPage(3)">Загрози та протидія</button>
        </div>

        <!-- Сторінка 1: Резюме -->
        <div class="page active" id="page1">
            <h2>Резюме</h2>
            
            <div class="resume-section">
                <h3>Особиста інформація</h3>
                <p><strong>Ім'я:</strong> Кнапець Валерія Андріївна</p>
                <p><strong>Дата народження:</strong> 25 липня 2007 року</p>
                <p><strong>Місце народження:</strong> Київ, Україна</p>
                <p><strong>Телефон:</strong> (+380) 953177328</p>
                <p><strong>Email:</strong> valeria.knapets@gmail.com</p>
            </div>

            <div class="resume-section">
                <h3>Освіта</h3>
                <p><strong>Період:</strong> 1 вересня 2014 – 24 травня 2025</p>
                <p><strong>Навчальний заклад:</strong> Ліцей "ГАРАНТ.ОСВІТА", Київ, Україна</p>
                <p><strong>Освітній рівень:</strong> Повна загальна середня освіта</p>
            </div>

            <div class="resume-section">
                <h3>Досвід роботи</h3>
                <p><strong>Посада:</strong> Менеджер класу</p>
                <p><strong>Період:</strong> 1 вересня 2022 – 31 травня 2024</p>
                <p><strong>Місце:</strong> Ліцей "ГАРАНТ.ОСВІТА", Київ</p>
                <p><strong>Обов'язки:</strong></p>
                <ul>
                    <li>Налагодження комунікації між учнями та вчителями</li>
                    <li>Допомога у знаходженні компромісів</li>
                    <li>Організація позакласних заходів</li>
                </ul>

                <p style="margin-top: 15px;"><strong>Посада:</strong> Художник-оформлювач</p>
                <p><strong>Період:</strong> 1 вересня 2023 – 25 травня 2025</p>
                <p><strong>Обов'язки:</strong> Допомога у створенні декорацій та оформленні приміщень для шкільних заходів</p>

                <p style="margin-top: 15px;"><strong>Посада:</strong> Няня</p>
                <p><strong>Період:</strong> з 1 березня 2023</p>
                <p><strong>Обов'язки:</strong> Догляд за дітьми родичів, приготування їжі для них</p>
            </div>

            <div class="resume-section">
                <h3>Мовні навички</h3>
                <p><strong>Рідна мова:</strong> Українська</p>
                <p><strong>Польська:</strong> B1 (розуміння), B1 (читання), A2 (усне мовлення та письмо)</p>
                <p><strong>Англійська:</strong> B2 (розуміння), B2 (читання), B1 (усне мовлення та письмо)</p>
            </div>

            <div class="resume-section">
                <h3>Волонтерство</h3>
                <p>Активна участь у волонтерських проєктах</p>
            </div>

            <div class="resume-section">
                <h3>Досягнення</h3>
                <p><strong>1 березня 2023:</strong> 3-тє місце у другому етапі Всеукраїнської учнівської олімпіади з права – Департамент освіти і науки</p>
            </div>
        </div>

        <!-- Сторінка 2: Економічна безпека -->
        <div class="page" id="page2">
            <h2>Економічна безпека Італії</h2>

            <div class="analysis-text">
                <p>Економіка Італії за останні 10 років демонструє повільне зростання з середнім темпом 0,5-1% на рік, що значно нижче середнього показника ЄС. Державний борг зріс зі 131% ВВП у 2014 році до 137% у 2024 році, залишаючись одним з найвищих у Європі. Інфляція коливалася від мінімуму 0,2% у 2016 році до піку 8,2% у 2022 році через енергетичну кризу, стабілізувавшись на рівні 2,6% у 2024 році. Енергетична залежність залишається критичною проблемою - протягом десятиліття країна імпортувала 74-79% енергії, найвищий показник серед великих європейських країн. Італія досягла прогресу у диверсифікації енергопостачання, знизивши залежність від російського газу з 41% у 2021 році до 3% у 2022 році. Основні виклики включають низьку продуктивність праці, високе податкове навантаження (42,8% ВВП) та необхідність модернізації економіки через реалізацію програми NRRP на €191,5 млрд від ЄС.</p>
            </div>

            <div class="chart-container">
                <h3>Ключові економічні показники Італії (2024)</h3>
                
                <div class="chart-bar">
                    <div class="chart-label">Державний борг (% ВВП)</div>
                    <div class="chart-bar-fill" style="width: 68.5%;">137%</div>
                </div>
                
                <div class="chart-bar">
                    <div class="chart-label">Темп зростання ВВП</div>
                    <div class="chart-bar-fill" style="width: 7%;">0,7%</div>
                </div>
                
                <div class="chart-bar">
                    <div class="chart-label">Інфляція</div>
                    <div class="chart-bar-fill" style="width: 26%;">2,6%</div>
                </div>
                
                <div class="chart-bar">
                    <div class="chart-label">Рівень безробіття</div>
                    <div class="chart-bar-fill" style="width: 60%;">6,0%</div>
                </div>
                
                <div class="chart-bar">
                    <div class="chart-label">Енергозалежність</div>
                    <div class="chart-bar-fill" style="width: 73.5%;">74,8%</div>
                </div>
            </div>

            <h3>Основні напрямки економічної політики</h3>
            <div class="analysis-text">
                <span class="indicator">Фіскальна консолідація</span>
                <span class="indicator">Цифрова трансформація</span>
                <span class="indicator">Зелений перехід</span>
                <span class="indicator">Підвищення продуктивності</span>
                <span class="indicator">Енергетична диверсифікація</span>
                <span class="indicator">Структурні реформи</span>
            </div>
        </div>

        <!-- Сторінка 3: Загрози та протидія -->
        <div class="page" id="page3">
            <h2>Загрози економічній безпеці Італії</h2>

            <div class="table-container">
                <div class="table-title">ЗАГРОЗИ ЕКОНОМІЧНІЙ БЕЗПЕЦІ</div>
                <table>
                    <thead>
                        <tr>
                            <th class="number-cell">№</th>
                            <th class="name-cell">Загроза</th>
                            <th>Поточний стан (динаміка за 10 років)</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td class="number-cell">1</td>
                            <td class="name-cell">Надмірний державний борг</td>
                            <td>Зростання з 131,1% ВВП (2014) до 137% ВВП (2024). Пік досягнув 157,7% у 2021 році під час пандемії. Середнє значення за десятиліття: 138% ВВП. Поточний борг: €2,97 трлн.</td>
                        </tr>
                        <tr>
                            <td class="number-cell">2</td>
                            <td class="name-cell">Енергетична залежність</td>
                            <td>Стабільно висока залежність: 75-82% імпорту енергії (2014-2024). У 2022 році: 79%, у 2024 році: 74,8%. Найвищий показник серед великих країн ЄС. Успішна диверсифікація: зниження імпорту з Росії з 41% (2021) до 3% (2022).</td>
                        </tr>
                        <tr>
                            <td class="number-cell">3</td>
                            <td class="name-cell">Корупція та організована злочинність</td>
                            <td>Індекс сприйняття корупції: 54/100 (2024), без значного покращення за десятиліття. Нижче середнього показника ЄС (64/100). Особливо гостра проблема в південних регіонах. Економічні втрати: орієнтовно €60-90 млрд щорічно.</td>
                        </tr>
                        <tr>
                            <td class="number-cell">4</td>
                            <td class="name-cell">Низька продуктивність праці</td>
                            <td>Стагнація продуктивності протягом 20+ років. Участь жінок на ринку праці: 52,8% (2024) - найнижча в ЄС. Середній ріст продуктивності: 0,2% на рік (2014-2024) проти 1,2% у середньому по ЄС. Демографічний спад: -5% працездатного населення за десятиліття.</td>
                        </tr>
                        <tr>
                            <td class="number-cell">5</td>
                            <td class="name-cell">Високе податкове навантаження</td>
                            <td>Податкові надходження: 42,8% ВВП (2023) - 3-тє місце серед країн ОЕСР. Стабільно високе протягом десятиліття: 42-44% ВВП. Податок на прибуток: 24%, ПДВ: 22%. Знижує конкурентоспроможність порівняно з Німеччиною (38,3%) та Францією (45,4%).</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <div class="table-container">
                <div class="table-title">МЕТОДИ ПРОТИДІЇ ЗАГРОЗАМ</div>
                <table>
                    <thead>
                        <tr>
                            <th class="number-cell">№</th>
                            <th class="name-cell">Метод протидії</th>
                            <th>Поточний стан (динаміка за 10 років)</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td class="number-cell">1</td>
                            <td class="name-cell">Фіскальна консолідація</td>
                            <td>Дефіцит бюджету знижується: з -3,0% ВВП (2014) до -3,6% ВВП (2024). Цільовий дефіцит: 2,6% ВВП до 2027 року. Первинний профіцит: досягнення 3% ВВП. Скасування програми Superbonus заощадить €18-20 млрд щорічно після 2024 року.</td>
                        </tr>
                        <tr>
                            <td class="number-cell">2</td>
                            <td class="name-cell">Диверсифікація енергетики</td>
                            <td>Відновлювальна енергія: зростання з 17% (2014) до 44% електрогенерації (2023). Нові газопроводи: TAP (Азербайджан, 10 млрд м³/рік), Transmed (Алжир, збільшення потужності). Зниження споживання газу: з 76 млрд м³ (2014) до 62 млрд м³ (2024). Інвестиції: €191,5 млрд від ЄС (NRRP).</td>
                        </tr>
                        <tr>
                            <td class="number-cell">3</td>
                            <td class="name-cell">Антикорупційна політика</td>
                            <td>Створення ANAC (2014), посилення контролю держзакупівель. Скорочення строків судових розглядів: з 1,190 днів (2014) до 527 днів (2024) для цивільних справ. Цифровізація держпослуг: 65% процедур онлайн (2024) проти 15% (2014). Відновлення активів: €8-12 млрд конфісковано за 2014-2024 рр.</td>
                        </tr>
                        <tr>
                            <td class="number-cell">4</td>
                            <td class="name-cell">Підвищення продуктивності та інновації</td>
                            <td>Фінансування NRRP: €191,5 млрд (2021-2026) на цифровізацію (27%), зелений перехід (37%), освіту (10%). Видатки на НДДКР: зростання з 1,29% ВВП (2014) до 1,47% ВВП (2023). Стартап-екосистема: 14,000+ стартапів (2024) проти 5,000 (2014). Інвестиції у вищу освіту: +15% реальних видатків за десятиліття.</td>
                        </tr>
                        <tr>
                            <td class="number-cell">5</td>
                            <td class="name-cell">Податкова реформа</td>
                            <td>Реформа IRPEF: об'єднання перших двох категорій (2024), зниження навантаження для доходів до €40,000. Податковий розрив: зменшення з €108 млрд (2014) до €83 млрд (2021) завдяки цифровізації. Електронне фактурування: обов'язкове з 2019 року, охоплення 95% операцій B2B. Зниження податку на бізнес: з 27,5% до 24% (2017).</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <div class="analysis-text" style="margin-top: 30px;">
                <h3>Висновок</h3>
                <p>Аналіз динаміки за останні 10 років показує, що Італія досягла прогресу в окремих сферах (диверсифікація енергетики, антикорупційні заходи), проте структурні проблеми державного боргу, низької продуктивності та податкового навантаження залишаються критичними викликами. Успішна реалізація програми NRRP та продовження структурних реформ є ключовими для довгострокової економічної безпеки країни.</p>
            </div>
        </div>
    </div>

    <script>
        function showPage(pageNum) {
            const pages = document.querySelectorAll('.page');
            const buttons = document.querySelectorAll('.nav-btn');
            
            pages.forEach(page => page.classList.remove('active'));
            buttons.forEach(btn => btn.classList.remove('active'));
            
            document.getElementById('page' + pageNum).classList.add('active');
            buttons[pageNum - 1].classList.add('active');
            
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }
    </script>
</body>
</html>
