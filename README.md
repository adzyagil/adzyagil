\documentclass[a4paper, 12pt]{article}
\usepackage[utf8]{inputenc}
\usepackage[russian]{babel}
\usepackage{enumitem}
\pagestyle{empty}
\usepackage{hyperref}
\usepackage{parskip}
\usepackage{xcolor}
\usepackage{amssymb}
\usepackage{fontspec}
\usepackage{fontawesome5}
\usepackage{tabularx} % в преамбуле, если ещё не подключён
\usepackage[left=1cm, right=1cm, top=1.5cm, bottom=1.5cm]{geometry}

% Настройки шрифтов
\setmainfont{EB Garamond} % или EB Garamond, Cormorant Garamond
\newfontfamily{\headingfont}{Cormorant Garamond SemiBold}
\linespread{1.05}

\definecolor{accent}{RGB}{0, 122, 255}
\definecolor{lightgray}{RGB}{200, 200, 200}

% Стили разделов
\usepackage{titlesec}
\titleformat{\section}{\headingfont\large\color{black}}{\thesection}{0em}{}[{\titlerule[0.8pt]}]
\titleformat{\subsection}{\headingfont\color{black}}{\thesubsection}{0em}{}

% Настройка списков
\setlist[itemize]{leftmargin=*, nosep, after=\vspace{0.5em}}
\setlist[enumerate]{leftmargin=*, nosep, after=\vspace{0.5em}}

\begin{document}

% --- Заголовок ---
\begin{center}
\noindent{\headingfont\Huge \textbf{Дзягиль Андрей Александрович}} \\
\vspace{0.5em}
\end{center}

% --- Контакты ---
\begin{center}
\faIcon{telegram} \href{https://t.me/electricfknwizart}{\textcolor{accent}{@electricfknwizart}} 
\textcolor{black}{\,|\,}
\faIcon{envelope} \href{mailto:adzyagil@yandex.ru}{\textcolor{accent}{adzyagil@yandex.ru}} 
\textcolor{black}{\,|\,}
\faIcon{mobile-alt} \href{tel:+79051200616}{\textcolor{accent}{+7 (905) 120-06-16}} 
\textcolor{black}{\,|\,}
\faIcon{github} \href{https://github.com/adzyagil}{\textcolor{accent}{GitHub}}
\end{center}


% --- О себе ---
\section*{ОБО МНЕ:}
Data Analyst с опытом работы с данными: от сбора и обработки до анализа и визуализации. Владею SQL, Python, Excel. Есть опыт построения статистических моделей, проведения исследований и работы с временными рядами. Интересуюсь аналитикой продукта и принятием решений на основе данных.

% --- Опыт работы ---
\section*{ОПЫТ}

\noindent
\begin{tabularx}{\textwidth}{Xr}
\textbf{ML Engineer, Проект: Domain Adaptation for Russian News Classification} & \textbf{Апрель 2025 — Июнь 2025} \\
\end{tabularx}

\begin{itemize}
    \item Исследовал переносимость моделей классификации новостей между доменами (Lenta.ru News, ~800k статей).
    \item Провел предобработку и анализ данных: очистка текстов, формирование обучающих и тестовых выборок, выделение признаков.
    \item Сравнил точность моделей при обучении на одном домене и применении к другому.
    \item Подготовил отчеты с результатами влияния доменной адаптации на качество классификации.
\end{itemize}

% --- Проекты ---
\section*{ПРОЕКТЫ}

\begin{itemize}
    \item \textbf{Классификация изображений (Kaggle):} построение пайплайна предобработки (кастомный Dataset, аугментации с Albumentations), эксперименты с архитектурами CNN: базовая модель, трансфер-лернинг на ResNet18, кастомная глубокая CNN. Реализован цикл обучения с OneCycleLR; метрика — accuracy. 
    
    \item \textbf{Мультилейбл классификация текстов (Kaggle):} задача многометочной классификации русскоязычных текстов (афиши/события). Реализованы разные подходы: TF-IDF + MLP, Word2Vec + линейная модель, CNN и BiLSTM, а также BERT. Предварительная очистка текста (лемматизация, удаление стоп-слов и эмодзи). Основная метрика — F1-score.
    
    \item \textbf{Анализ временных рядов:} исследование взаимосвязи индекса Московской биржи и динамики денежной массы. Построение моделей SARIMA, VAR и интерпретация полученных функций откликов.
    
    \item \textbf{Исследование зарплат для нескольких регионов:} анализ факторов, влияющих на гендерный разрыв в оплате труда. Построение линейных моделей, проведение статистических тестов и интерпретация полученных коэффициентов.
\end{itemize}

% --- Образование ---
\section*{ОБРАЗОВАНИЕ}
\noindent
\begin{tabularx}{\textwidth}{@{}Xr@{}}
\textbf{РАНХиГС, бакалавриат} & \textbf{4 курс} \\
\end{tabularx}
Институт экономики, математики и информационных технологий. Отделение экономики. Образовательная программа "Цифровая экономика"

% --- Навыки ---
\section*{НАВЫКИ}
\begin{itemize}
    \item \textbf{Анализ данных:} SQL (PostgreSQL, MySQL), Excel, Pandas, NumPy
    \item \textbf{Визуализация и BI:} Matplotlib, Seaborn, Tableau, Plotly
    \item \textbf{Статистика:} A/B-тестирование, z-test, t-test, MDE, регрессионный анализ, временные ряды
    \item \textbf{Машинное обучение:} Scikit-learn, CatBoost, PyTorch
    \item \textbf{NLP и CV:} NLTK, BERT, SentenceTransformers, EfficientNet, Albumentations
    \item \textbf{Иностранные языки:} Английский (B2)
\end{itemize}

\end{document}
