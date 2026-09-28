<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover" />
  <title>probschool</title>
  <meta name="description" content="ProbSchool (probschool.kz) — поиск школ и сообщения о проблемах школы. Автор: Т.Оразәлі." />
  <meta name="author" content="Т.Оразәлі" />
  <meta name="keywords" content="probschool, probschool.kz, проблемы школы, поиск школы, Караганда" />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --bg: #0d1220;
      --panel: #1a1f2e;
      --field: #2b3144;
      --field-hover: #343b52;
      --text: #f2f4f8;
      --muted: #9aa3b8;
      --gold: #e8d36a;
      --accent: #c57a1a;
      --accent-hover: #d88920;
      --danger: #e07a8a;
      --blue: #3b82f6;
      --border: #3a4158;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    html, body { background: var(--bg); color: var(--text); font-family: Inter, system-ui, sans-serif; min-height: 100%; }
    body { padding-bottom: 24px; padding-top: 52px; }

    .topbar {
      display: flex; align-items: center; justify-content: center;
      padding: 12px 16px; background: #1a1f2c;
      border-bottom: 1px solid #2a3144;
      position: fixed; top: 0; left: 0; right: 0; z-index: 50;
    }
    .brand {
      font-weight: 700; font-size: 17px; color: #fff; letter-spacing: 0.3px;
      background: #2b3144; border-radius: 999px; padding: 8px 18px; min-width: 70%;
      text-align: center;
    }
    .brand span { color: var(--gold); font-weight: 700; }
    .lang { color: var(--muted); font-size: 14px; letter-spacing: 0.5px; }
    .lang span { margin: 0 6px; cursor: pointer; }
    .lang span.active { color: #fff; }

    .wrap { padding: 18px 16px 0; max-width: 560px; margin: 0 auto; }
    .page { display: none; }
    .page.show { display: block; }
    h2 { font-size: 26px; font-weight: 600; margin: 8px 0 14px; }
    h3 { font-size: 24px; font-weight: 600; margin: 22px 0 8px; }

    .card {
      background: var(--panel); border-radius: 12px; padding: 16px 14px 18px;
      box-shadow: 0 8px 24px rgba(0,0,0,.25);
    }
    label.lbl { display: block; font-size: 14px; color: #d5dae6; margin: 12px 0 6px; }
    label.lbl:first-child { margin-top: 0; }

    .select-btn, .combo input {
      width: 100%; background: var(--field); border: none; color: var(--text);
      border-radius: 8px; padding: 12px 40px 12px 14px; font-size: 15px; min-height: 46px;
    }
    .select-btn { text-align: left; position: relative; cursor: pointer; }
    .select-btn::after, .combo .chev {
      content: "▾"; position: absolute; right: 14px; top: 50%; transform: translateY(-50%);
      color: #c5c9d6; font-size: 12px; pointer-events: none;
    }
    .select-btn:hover { background: var(--field-hover); }
    .combo { position: relative; }
    .combo input { outline: none; }
    .combo input::placeholder { color: #7d8699; }

    .dropdown {
      display: none; position: absolute; left: 0; right: 0; top: calc(100% + 4px);
      background: #2a3144; border-radius: 10px; max-height: 260px; overflow-y: auto;
      z-index: 20; box-shadow: 0 12px 32px rgba(0,0,0,.45); border: 1px solid var(--border);
    }
    .dropdown.open { display: block; }
    .dropdown .opt { padding: 12px 14px; cursor: pointer; font-size: 14px; border-bottom: 1px solid rgba(255,255,255,.04); }
    .dropdown .opt:hover { background: #3a4560; }
    .dropdown .opt small { display: block; color: var(--muted); font-size: 12px; margin-top: 2px; }
    .dropdown .empty-msg { padding: 14px; color: var(--muted); font-size: 13px; }

    .actions { display: flex; gap: 10px; margin-top: 16px; }
    .btn { border: none; border-radius: 8px; padding: 11px 16px; font-size: 15px; font-weight: 600; cursor: pointer; }
    .btn-search { background: var(--accent); color: #fff; }
    .btn-search:hover { background: var(--accent-hover); }
    .btn-reset { background: transparent; color: var(--danger); border: 1.5px solid #8a3a48; }

    .count { color: var(--muted); font-size: 13px; margin-bottom: 10px; }
    .results { display: flex; flex-direction: column; gap: 10px; }
    .school { background: var(--panel); border-radius: 12px; padding: 14px; cursor: pointer; border: 1px solid transparent; }
    .school:hover { border-color: #4a5570; background: #22283a; }
    .school .go { margin-top: 8px; font-size: 13px; color: var(--gold); }
    .school .name { font-size: 15px; font-weight: 600; line-height: 1.35; margin-bottom: 8px; }
    .meta { font-size: 13px; color: var(--muted); display: grid; gap: 3px; }
    .meta b { color: #cfd6e6; font-weight: 500; }
    .tag { display: inline-block; margin-top: 8px; background: #24324a; color: #9ec5ff; font-size: 12px; padding: 3px 8px; border-radius: 999px; }

    .overlay {
      display: none; position: fixed; inset: 0; background: rgba(0,0,0,.55);
      z-index: 40; align-items: flex-end; justify-content: center;
    }
    .overlay.show { display: flex; }
    .sheet {
      background: #2a2f3d; width: min(480px, 100%); max-height: 86vh;
      border-radius: 18px 18px 0 0; padding: 12px 0 20px; display: flex; flex-direction: column;
    }
    .sheet-top { display: flex; justify-content: flex-end; gap: 8px; padding: 4px 14px 8px; }
    .mini { background: #3a4154; color: #ddd; border: none; border-radius: 8px; padding: 7px 12px; font-size: 13px; cursor: pointer; }
    .mini.primary { background: #1e1e26; color: #fff; }
    .sheet-search { padding: 0 14px 8px; }
    .sheet-search input {
      width: 100%; background: #1c2130; border: 1px solid var(--border); color: #fff;
      border-radius: 8px; padding: 10px 12px; font-size: 15px; outline: none;
    }
    .sheet-list { overflow-y: auto; padding: 4px 8px 8px; }
    .radio { display: flex; align-items: center; gap: 12px; padding: 13px 14px; cursor: pointer; font-size: 16px; }
    .radio .dot {
      width: 22px; height: 22px; border-radius: 50%; border: 2px solid #7a8296; flex-shrink: 0; position: relative;
    }
    .radio.checked .dot { border-color: var(--blue); }
    .radio.checked .dot::after {
      content: ""; position: absolute; inset: 4px; border-radius: 50%; background: var(--blue);
    }
    .done { text-align: center; padding: 12px; font-size: 16px; color: #eee; cursor: pointer; }

    .hint { margin-top: 10px; font-size: 12px; color: var(--muted); line-height: 1.4; }
    .author {
      margin: 28px 0 10px; text-align: center; padding: 16px 12px;
      border-top: 1px solid #2a3144;
    }
    .author .mark {
      font-size: 22px; font-weight: 700; letter-spacing: 0.5px; color: var(--gold);
    }
    .author .sub { margin-top: 4px; font-size: 12px; color: #6d7588; }

    .back {
      background: none; border: none; color: #9ec5ff; font-size: 15px;
      cursor: pointer; margin-bottom: 10px; padding: 0;
    }
    textarea.area {
      width: 100%; min-height: 160px; background: var(--field); border: none;
      color: var(--text); border-radius: 8px; padding: 12px 14px; font-size: 15px;
      font-family: inherit; outline: none; resize: vertical;
    }
    .ok { display: none; margin-top: 12px; color: #8fd19e; font-size: 14px; }
    .reports { margin-top: 16px; display: flex; flex-direction: column; gap: 8px; }
    .report-item { background: #22283a; border-radius: 10px; padding: 12px; font-size: 14px; }
    .report-item time { display: block; color: var(--muted); font-size: 12px; margin-bottom: 4px; }
  </style>
</head>
<body>
  <div class="topbar">
    <div class="brand">probschool</div>
  </div>

  <main class="wrap">
    <section class="page show" id="pageSearch">
    <h2>ProbSchool</h2>
    <p class="hint" style="margin: -6px 0 14px">Сайт: <b style="color:#e8d36a">probschool.kz</b> · поиск: <b>probschool</b></p>
    <p class="hint" style="margin: 0 0 14px">Здесь много школ Карагандинской области и примеры по другим регионам. Все школы Казахстана (около 5100) есть только на официальном сайте portal.mektebi.kz.</p>

    <form class="card" id="searchForm" onsubmit="return doSearch(event)">
      <label class="lbl">Регионы:</label>
      <button type="button" class="select-btn" id="regionBtn" onclick="openRegionPicker()">Карагандинская область</button>

      <label class="lbl">Районы:</label>
      <button type="button" class="select-btn" id="districtBtn" onclick="openDistrictPicker()">Все районы</button>

      <label class="lbl">Наименование организации:</label>
      <div class="combo">
        <input id="schoolInput" type="text" placeholder="Выберите или начните вводить название" autocomplete="off"
               onfocus="openSchoolDrop()" oninput="filterSchools()" />
        <span class="chev">▾</span>
        <div class="dropdown" id="schoolDrop"></div>
      </div>

      <label class="lbl">БИН:</label>
      <div class="combo">
        <input id="binInput" type="text" placeholder="Можно выбрать из списка" autocomplete="off"
               onfocus="openBinDrop()" oninput="filterBins()" />
        <span class="chev">▾</span>
        <div class="dropdown" id="binDrop"></div>
      </div>

      <label class="lbl">Форма управления:</label>
      <button type="button" class="select-btn" id="formBtn" onclick="openFormPicker()">Государственное</button>

      <div class="actions">
        <button class="btn btn-search" type="submit">🔍 Искать</button>
        <button class="btn btn-reset" type="button" onclick="resetForm()">✕ Сброс</button>
      </div>
      <p class="hint">Напишите «крг» или выберите Карагандинскую область — сразу появятся все школы области. Район можно не выбирать.</p>
    </form>

    <h3>Школы</h3>
    <p class="count" id="count"></p>
    <div class="results" id="results"></div>

    <footer class="author">
      <div class="mark">Т.Оразәлі</div>
      <div class="sub">Автор страницы. Копирование без указания имени запрещено.</div>
    </footer>
    </section>

    <section class="page" id="pageReport">
      <button class="back" type="button" onclick="backToList()">← Назад к школам</button>
      <h2>Проблема школы</h2>
      <div class="card" style="margin-bottom:14px">
        <div class="name" id="repSchoolName" style="font-weight:600;margin-bottom:6px"></div>
        <div class="meta">
          <div>Район / город: <b id="repDistrict"></b></div>
          <div>Регион: <b id="repRegion"></b></div>
        </div>
      </div>
      <form class="card" onsubmit="return saveProblem(event)">
        <label class="lbl">Ваше имя (необязательно)</label>
        <input class="combo" id="repAuthor" type="text" value="" placeholder="Можно не писать" style="width:100%;background:var(--field);border:none;color:var(--text);border-radius:8px;padding:12px 14px;font-size:15px;min-height:46px" />
        <label class="lbl">Что случилось в школе?</label>
        <textarea class="area" id="repText" placeholder="Напишите проблему: ремонт, отопление, питание, безопасность, уроки..."></textarea>
        <div class="actions">
          <button class="btn btn-search" type="submit">Отправить</button>
          <button class="btn btn-reset" type="button" onclick="backToList()">Отмена</button>
        </div>
        <p class="ok" id="repOk">Запись сохранена на этом устройстве.</p>
      </form>
      <h3>Ранее написанные проблемы</h3>
      <div class="reports" id="repList"></div>
      <footer class="author">
        <div class="mark">Т.Оразәлі</div>
        <div class="sub">Автор страницы. Копирование без указания имени запрещено.</div>
      </footer>
    </section>
  </main>

  <div class="overlay" id="overlay" onclick="if(event.target===this) closePicker()">
    <div class="sheet">
      <div class="sheet-top">
        <button class="mini" type="button" onclick="closePicker()">Назад</button>
        <button class="mini primary" type="button" onclick="closePicker()">Далее</button>
      </div>
      <div class="sheet-search" id="sheetSearchWrap">
        <input id="sheetSearch" type="text" placeholder="Найти: крг, караганда..." oninput="filterPicker()" />
      </div>
      <div class="sheet-list" id="sheetList"></div>
      <div class="done" onclick="closePicker()">Готово</div>
    </div>
  </div>

  <script>
    const ALL = "Все районы";
    const FORMS = ["Все формы", "Государственное", "Частное"];

    const ALIASES = {
      "Карагандинская область": ["крг", "крг область", "караганда", "карагандинская", "карагандинская область", "qaragandy", "karaganda", "қарағанды", "қарағанды облысы"],
      "г. Астана": ["астана", "нур-султан", "astana"],
      "г. Алматы": ["алматы", "алма-ата", "almaty"],
      "г. Шымкент": ["шымкент", "chimkent"],
      "Костанайская область": ["кст", "костанай"],
      "Павлодарская область": ["павлодар"],
      "Акмолинская область": ["акмола", "кокшетау"],
    };

    function s(name, district, head) {
      return { name, district, head: head || "—", bin: "—" };
    }

    const KRG = [
      s("Гимназия №1", "г. Караганда", "Шнель Татьяна Ивановна"),
      s("Лицей №2", "г. Караганда", "Абзалиева Корлан Жамсаповна"),
      s("Гимназия №3", "г. Караганда", "Кульжамбекова Сауле Кажыкеримовна"),
      s("Общеобразовательная школа №4", "г. Караганда"),
      s("Школа-центр дополнительного образования №5", "г. Караганда"),
      s("Общеобразовательная школа №6", "г. Караганда"),
      s("Общеобразовательная школа №8", "г. Караганда"),
      s("Гимназия №9 имени Казыбека Нуржанова", "г. Караганда", "Бартош Светлана Николаевна"),
      s("Общеобразовательная школа №10", "г. Караганда"),
      s("Основная средняя школа №11", "г. Караганда"),
      s("Общеобразовательная школа №12", "г. Караганда"),
      s("Общеобразовательная школа №15", "г. Караганда"),
      s("Общеобразовательная школа №16", "г. Караганда"),
      s("Общеобразовательная школа №17", "г. Караганда"),
      s("Общеобразовательная школа №18", "г. Караганда"),
      s("Основная средняя школа №20", "г. Караганда"),
      s("Основная средняя школа №21", "г. Караганда"),
      s("Общеобразовательная школа №23", "г. Караганда"),
      s("Общеобразовательная школа №25", "г. Караганда"),
      s("Общеобразовательная школа №27", "г. Караганда"),
      s("Общеобразовательная школа №30", "г. Караганда"),
      s("Общеобразовательная школа №32", "г. Караганда"),
      s("Комплекс школа-ясли-сад №33", "г. Караганда"),
      s("Общеобразовательная школа №34", "г. Караганда"),
      s("Общеобразовательная школа №35 им. Ю.Н. Павлова", "г. Караганда"),
      s("Общеобразовательная школа №36", "г. Караганда"),
      s("Основная средняя школа №37", "г. Караганда"),
      s("Гимназия №38 имени Каныша Сатпаева", "г. Караганда", "Нурмуханов Бейбит Насиболлаевич"),
      s("Гимназия №39 имени Магжана Жумабаева", "г. Караганда", "Жалелов Абылай Армияұлы"),
      s("Основная средняя школа №40", "г. Караганда"),
      s("Школа-гимназия №41 имени Ахмета Байтурсынулы", "г. Караганда", "Жакаева Самал Сансызбаевна"),
      s("Основная школа №42", "г. Караганда"),
      s("Основная средняя школа №44", "г. Караганда"),
      s("Гимназия №45", "г. Караганда", "Жарасова Елена Викторовна"),
      s("Общеобразовательная школа №46", "г. Караганда"),
      s("Общеобразовательная школа №48", "г. Караганда"),
      s("Общеобразовательная школа №50", "г. Караганда"),
      s("Общеобразовательная школа №52 им. академика Е.А. Букетова", "г. Караганда"),
      s("Школа-лицей №53", "г. Караганда", "Садвакасова Айман Дарменовна"),
      s("Общеобразовательная школа №54", "г. Караганда"),
      s("Основная средняя школа №56", "г. Караганда"),
      s("Школа-лицей №57 имени С. Саттарова", "г. Караганда", "Сейтимбетова Куланшаш Төлекқызы"),
      s("Общеобразовательная школа №58 им. Нуркена Абдирова", "г. Караганда"),
      s("Общеобразовательная школа №59", "г. Караганда"),
      s("Общеобразовательная школа №60", "г. Караганда"),
      s("Общеобразовательная школа №61", "г. Караганда"),
      s("Общеобразовательная школа №62", "г. Караганда"),
      s("Общеобразовательная школа №63", "г. Караганда"),
      s("Основная средняя школа №64", "г. Караганда"),
      s("Общеобразовательная школа №65", "г. Караганда"),
      s("Школа-лицей №66", "г. Караганда", "Мисюрина Наталья Михайловна"),
      s("Общеобразовательная школа №74", "г. Караганда"),
      s("Общеобразовательная школа №76 им. Алихана Бокейхана", "г. Караганда"),
      s("Общеобразовательный комплекс школа-детский сад №77 им. Бауыржана Момышулы", "г. Караганда"),
      s("Основная средняя школа №78", "г. Караганда"),
      s("Основная средняя школа №79", "г. Караганда"),
      s("Общеобразовательная школа №81", "г. Караганда"),
      s("Общеобразовательная школа №82", "г. Караганда"),
      s("Общеобразовательная школа №83 им. Г. Мустафина", "г. Караганда"),
      s("Общеобразовательная школа №85", "г. Караганда"),
      s("Общеобразовательная школа №86", "г. Караганда"),
      s("Основная средняя школа №87", "г. Караганда"),
      s("Общеобразовательная школа №88", "г. Караганда"),
      s("Общеобразовательная школа №91", "г. Караганда"),
      s("Гимназия №92 имени Сакена Сейфуллина", "г. Караганда", "Жунусова Салтанат Оразбаевна"),
      s("Гимназия №93 имени Шакарима", "г. Караганда", "Ахметова Аягуль Нурабаевна"),
      s("Школа-гимназия №95", "г. Караганда"),
      s("Гимназия №97", "г. Караганда"),
      s("Вечерняя школа №100", "г. Караганда"),
      s("Школа-лицей №101", "г. Караганда"),
      s("Основная средняя школа №134", "г. Караганда"),
      s("Основная средняя школа №137", "г. Караганда"),
      s("Школа-гимназия имени Абая", "г. Караганда"),
      s("Школа-гимназия имени Аль-Фараби", "г. Караганда"),
      s("Школа-лицей имени Алимхана Ермекова", "г. Караганда"),
      s("Специализированная школа-интернат Мурагер", "г. Караганда"),
      s("Специализированная школа-интернат имени Н. Нурмакова", "г. Караганда"),
      s("Специализированная музыкальная школа-интернат", "г. Караганда"),
      s("Специализированная школа-интернат Дарын", "г. Караганда"),
      s("Лицей-интернат Білім-Инновация №1", "г. Караганда"),
      s("Лицей-интернат Білім-Инновация №2", "г. Караганда"),

      s("Общеобразовательная школа №1", "г. Темиртау"),
      s("Общеобразовательная школа №2", "г. Темиртау"),
      s("Общеобразовательная школа №3", "г. Темиртау"),
      s("Общеобразовательная школа №4", "г. Темиртау"),
      s("Общеобразовательная школа №5 им. Габидена Мустафина", "г. Темиртау"),
      s("Общеобразовательная школа №6", "г. Темиртау"),
      s("Общеобразовательная школа №7", "г. Темиртау"),
      s("Общеобразовательная школа №8", "г. Темиртау"),
      s("Лицей №9", "г. Темиртау"),
      s("Общеобразовательная школа №10", "г. Темиртау"),
      s("Средняя общеобразовательная школа №11", "г. Темиртау"),
      s("Школа №12", "г. Темиртау"),
      s("Школа №16", "г. Темиртау"),
      s("Школа №17", "г. Темиртау"),
      s("Школа №19", "г. Темиртау"),
      s("Лицей №20", "г. Темиртау"),
      s("Школа №21", "г. Темиртау"),
      s("Общеобразовательная школа №22", "г. Темиртау"),
      s("Школа №23", "г. Темиртау"),
      s("Общеобразовательная школа №24", "г. Темиртау"),
      s("Школа №27", "г. Темиртау"),
      s("Общеобразовательная школа №31", "г. Темиртау"),
      s("Гимназия имени Т. Аубакирова", "г. Темиртау"),
      s("Женская гимназия", "г. Темиртау"),

      s("Средняя школа №4", "г. Балхаш"),
      s("Средняя школа №9", "г. Балхаш"),
      s("Общеобразовательная школа имени Аль-Фараби", "г. Балхаш"),
      s("Общеобразовательная школа №12", "г. Балхаш"),

      s("Средняя школа №3", "г. Сарань"),
      s("Школа-гимназия №17", "г. Сарань"),

      s("Гимназия №1", "г. Шахтинск"),
      s("Общеобразовательная школа №2", "г. Шахтинск"),
      s("Общеобразовательная школа №3", "г. Шахтинск"),
      s("Общеобразовательная школа №4", "г. Шахтинск"),
      s("Гимназия №5", "г. Шахтинск"),
      s("Школа-гимназия имени Сакена Сейфуллина", "г. Шахтинск"),
      s("Школа-лицей имени Әлихана Бөкейханова", "г. Шахтинск"),

      s("Казахская средняя общеобразовательная школа №1 (опорная)", "Бухар-Жырауский район", "Тургумбаева Бадиша Мукушевна"),
      s("Токаревская средняя общеобразовательная школа", "Бухар-Жырауский район", "Макаров Мереке Ескендирович"),
      s("Кушокинская средняя общеобразовательная школа", "Бухар-Жырауский район"),
      s("Средняя школа села Ботакара", "Бухар-Жырауский район"),
      s("Общеобразовательная школа имени Абая села Гагаринское", "Бухар-Жырауский район"),
      s("Основная школа села Уштобе", "Бухар-Жырауский район"),

      s("Средняя школа города Абай №1", "Абайский район"),
      s("Школа-гимназия города Абай", "Абайский район"),
      s("Средняя школа имени Абая, посёлок Топар", "Абайский район"),
      s("Средняя школа имени Момышұлы, посёлок Топар", "Абайский район"),
      s("Есенгельдинская общеобразовательная школа", "Абайский район"),
      s("Дзержинская общеобразовательная школа села Сарепта", "Абайский район"),

      s("Общеобразовательная средняя школа посёлка Сарышаган", "Актогайский район"),
      s("Средняя школа села Актогай", "Актогайский район"),
      s("Общеобразовательная школа имени Жабас Кеңесбаева, село Сартерек", "Актогайский район"),

      s("Средняя школа имени Бухар жырау, г. Каркаралинск", "Каркаралинский район"),
      s("СОШ №22 села Томар", "Каркаралинский район", "Бекбосын Алмас Қабдоллаұлы"),
      s("СОШ №23 села Татан", "Каркаралинский район", "Рахымбеков Мейрам Жакыбаевич"),
      s("Основная школа №24 села Акбай-Кызылбай", "Каркаралинский район"),
      s("Начальная школа №25 села Аккора", "Каркаралинский район"),
      s("Средняя школа села Талды", "Каркаралинский район"),

      s("Средняя школа села Киевка", "Нуринский район"),
      s("Опорная школа (гимназия №9) посёлка Осакаровка", "Осакаровский район"),
      s("Средняя школа №1 посёлка Осакаровка", "Осакаровский район"),
      s("Средняя школа села Аксу-Аюлы", "Шетский район"),
      s("Школа посёлка имени Сакена Сейфуллина", "Шетский район", "Алма Абеуова")
    ];

    const DATA = {
      "г. Астана": [
        s("Школа-гимназия №31", "г. Астана", "Чужетова Айнур Сапаргалиевна"),
        s("Школа-лицей №1 имени Талгата Бигельдинова", "г. Астана"),
        s("Средняя школа №72", "г. Астана")
      ],
      "г. Алматы": [
        s("Гимназия №25", "Алмалинский район"),
        s("Специализированный лицей №165", "Бостандыкский район")
      ],
      "г. Шымкент": [
        s("Общеобразовательная школа №45", "Аль-Фарабийский район")
      ],
      "Акмолинская область": [
        s("Основная средняя школа села Айдарлы", "Зерендинский район"),
        s("Общеобразовательная школа села Акадыр", "Зерендинский район")
      ],
      "Актюбинская область": [s("Школа-гимназия №21", "г. Актобе")],
      "Алматинская область": [s("Средняя школа №5 села Отеген батыр", "Илийский район")],
      "Атырауская область": [s("Школа-лицей №8", "г. Атырау")],
      "Западно-Казахстанская область": [s("Средняя школа №12", "г. Уральск")],
      "Жамбылская область": [s("Гимназия имени Жамбыла", "г. Тараз")],
      "Карагандинская область": KRG,
      "Костанайская область": [s("Гимназия имени Ы. Алтынсарина", "г. Костанай")],
      "Кызылординская область": [s("Школа-лицей №10", "г. Кызылорда")],
      "Мангистауская область": [s("Средняя школа №6", "г. Актау")],
      "Павлодарская область": [s("Гимназия №3", "г. Павлодар")],
      "Северо-Казахстанская область": [s("Школа-гимназия №1", "г. Петропавловск")],
      "Восточно-Казахстанская область": [s("Лицей №44", "г. Усть-Каменогорск")],
      "Туркестанская область": [s("Средняя школа имени Яссауи", "г. Туркестан")],
      "Абайская область": [
        s("Средняя школа-сад имени Бауыржана Жунисова", "Уржарский район"),
        s("Школа-гимназия №3", "г. Семей")
      ],
      "Жетысуская область": [s("Гимназия №2", "г. Талдыкорган")],
      "Улытауская область": [s("Средняя школа №1", "г. Жезказган")]
    };

    const REGIONS = Object.keys(DATA);

    let state = {
      region: "Карагандинская область",
      district: ALL,
      form: "Государственное",
      picker: null,
      pickerItems: []
    };

    function districtsOf(region) {
      const set = new Set((DATA[region] || []).map(x => x.district));
      return [ALL, ...[...set]];
    }

    function schoolsOf() {
      let list = DATA[state.region] || [];
      if (state.district && state.district !== ALL) {
        list = list.filter(x => x.district === state.district);
      }
      return list;
    }

    function matchAlias(region, q) {
      if (!q) return true;
      const low = q.toLowerCase();
      if (region.toLowerCase().includes(low)) return true;
      return (ALIASES[region] || []).some(a => a.includes(low) || low.includes(a));
    }

    function openPicker(type) {
      state.picker = type;
      document.getElementById("sheetSearch").value = "";
      document.getElementById("sheetSearchWrap").style.display = type === "form" ? "none" : "block";
      document.getElementById("sheetSearch").placeholder =
        type === "region" ? "Найти: крг, караганда..." : "Найти район...";
      fillPicker();
      document.getElementById("overlay").classList.add("show");
      if (type !== "form") setTimeout(() => document.getElementById("sheetSearch").focus(), 50);
    }
    function openRegionPicker() { openPicker("region"); }
    function openDistrictPicker() { openPicker("district"); }
    function openFormPicker() { openPicker("form"); }

    function fillPicker() {
      const q = document.getElementById("sheetSearch").value.trim();
      const list = document.getElementById("sheetList");
      list.innerHTML = "";
      let items = [];
      let current = "";
      if (state.picker === "region") {
        items = REGIONS.filter(r => matchAlias(r, q));
        current = state.region;
      }
      if (state.picker === "district") {
        items = districtsOf(state.region).filter(d => !q || d.toLowerCase().includes(q.toLowerCase()));
        current = state.district;
      }
      if (state.picker === "form") { items = FORMS; current = state.form; }
      state.pickerItems = items;
      if (!items.length) {
        list.innerHTML = '<div class="empty-msg" style="padding:14px;color:#9aa3b8">Ничего не найдено</div>';
        return;
      }
      items.forEach(item => {
        const row = document.createElement("div");
        row.className = "radio" + (item === current ? " checked" : "");
        row.innerHTML = `<span class="dot"></span><span>${item}</span>`;
        row.onclick = () => pick(state.picker, item);
        list.appendChild(row);
      });
    }
    function filterPicker() { fillPicker(); }

    function pick(type, value) {
      if (type === "region") {
        state.region = value;
        state.district = ALL;
        document.getElementById("regionBtn").textContent = value;
        document.getElementById("districtBtn").textContent = ALL;
        document.getElementById("schoolInput").value = "";
        document.getElementById("binInput").value = "";
        renderResults(schoolsOf());
      }
      if (type === "district") {
        state.district = value;
        document.getElementById("districtBtn").textContent = value;
        document.getElementById("schoolInput").value = "";
        document.getElementById("binInput").value = "";
        renderResults(schoolsOf());
      }
      if (type === "form") {
        state.form = value;
        document.getElementById("formBtn").textContent = value;
      }
      closePicker();
    }
    function closePicker() {
      document.getElementById("overlay").classList.remove("show");
    }

    function renderDrop(el, items, onPick, emptyText) {
      if (!items.length) {
        el.innerHTML = `<div class="empty-msg">${emptyText}</div>`;
      } else {
        el.innerHTML = items.map((sch, i) =>
          `<div class="opt" data-i="${i}"><div>${sch.name}</div><small>${sch.district}</small></div>`
        ).join("");
        el.querySelectorAll(".opt").forEach(opt => {
          opt.onclick = () => onPick(items[+opt.dataset.i]);
        });
      }
      el.classList.add("open");
    }

    function openSchoolDrop() {
      const q = document.getElementById("schoolInput").value.trim().toLowerCase();
      const list = schoolsOf().filter(sch => !q || sch.name.toLowerCase().includes(q));
      renderDrop(document.getElementById("schoolDrop"), list.slice(0, 40), selectSchool, "Школ не найдено");
    }
    function filterSchools() { openSchoolDrop(); }

    function openBinDrop() {
      const q = document.getElementById("binInput").value.trim().toLowerCase();
      const list = schoolsOf().filter(sch => !q || sch.name.toLowerCase().includes(q) || String(sch.bin).includes(q));
      renderDrop(document.getElementById("binDrop"), list.slice(0, 40), selectSchool, "Не найдено");
    }
    function filterBins() { openBinDrop(); }

    function selectSchool(sch) {
      document.getElementById("schoolInput").value = sch.name;
      document.getElementById("binInput").value = sch.bin === "—" ? "" : sch.bin;
      document.getElementById("schoolDrop").classList.remove("open");
      document.getElementById("binDrop").classList.remove("open");
    }

    document.addEventListener("click", (e) => {
      if (!e.target.closest(".combo")) {
        document.getElementById("schoolDrop").classList.remove("open");
        document.getElementById("binDrop").classList.remove("open");
      }
    });

    function doSearch(ev) {
      ev.preventDefault();
      let list = schoolsOf();
      const qName = document.getElementById("schoolInput").value.trim().toLowerCase();
      if (qName) list = list.filter(sch => sch.name.toLowerCase().includes(qName));
      renderResults(list);
      return false;
    }

    function renderResults(list) {
      const box = document.getElementById("results");
      document.getElementById("count").textContent = list.length
        ? `Найдено школ: ${list.length}  ·  ${state.region}${state.district !== ALL ? " · " + state.district : ""}`
        : "Ничего не найдено.";
      box.innerHTML = list.map((sch, i) => `
        <article class="school" onclick='openReport(${JSON.stringify(sch.name)}, ${JSON.stringify(sch.district)})'>
          <div class="name">${i + 1}. ${sch.name}</div>
          <div class="meta">
            <div>Район / город: <b>${sch.district}</b></div>
            <div>Руководитель: <b>${sch.head}</b></div>
            <div>Регион: <b>${state.region}</b></div>
          </div>
          <span class="tag">${state.form === "Все формы" ? "Государственное" : state.form}</span>
          <div class="go">Нажать → написать проблему школы</div>
        </article>
      `).join("");
    }

    let currentSchool = null;

    function keyFor(name, district) {
      return "school-problems:" + state.region + "|" + district + "|" + name;
    }

    function openReport(name, district) {
      currentSchool = { name, district, region: state.region };
      document.getElementById("repSchoolName").textContent = name;
      document.getElementById("repDistrict").textContent = district;
      document.getElementById("repRegion").textContent = state.region;
      document.getElementById("repText").value = "";
      document.getElementById("repOk").style.display = "none";
      document.getElementById("pageSearch").classList.remove("show");
      document.getElementById("pageReport").classList.add("show");
      window.scrollTo(0, 0);
      drawReports();
    }

    function backToList() {
      document.getElementById("pageReport").classList.remove("show");
      document.getElementById("pageSearch").classList.add("show");
      window.scrollTo(0, 0);
    }

    function loadReports() {
      if (!currentSchool) return [];
      try {
        return JSON.parse(localStorage.getItem(keyFor(currentSchool.name, currentSchool.district)) || "[]");
      } catch (e) { return []; }
    }

    function drawReports() {
      const items = loadReports();
      const box = document.getElementById("repList");
      if (!items.length) {
        box.innerHTML = '<p class="count">Пока нет записей по этой школе.</p>';
        return;
      }
      box.innerHTML = items.map(r => `
        <div class="report-item">
          <time>${r.when} · ${r.author || "Анонимно"}</time>
          ${r.text}
        </div>
      `).join("");
    }

    function saveProblem(ev) {
      ev.preventDefault();
      const text = document.getElementById("repText").value.trim();
      if (!text) {
        document.getElementById("repText").focus();
        return false;
      }
      const items = loadReports();
      items.unshift({
        text,
        author: document.getElementById("repAuthor").value.trim() || "Анонимно",
        when: new Date().toLocaleString("ru-RU")
      });
      localStorage.setItem(keyFor(currentSchool.name, currentSchool.district), JSON.stringify(items));
      document.getElementById("repText").value = "";
      document.getElementById("repOk").style.display = "block";
      drawReports();
      return false;
    }

    function resetForm() {
      state.region = "Карагандинская область";
      state.district = ALL;
      state.form = "Государственное";
      document.getElementById("regionBtn").textContent = state.region;
      document.getElementById("districtBtn").textContent = ALL;
      document.getElementById("formBtn").textContent = state.form;
      document.getElementById("schoolInput").value = "";
      document.getElementById("binInput").value = "";
      renderResults(schoolsOf());
    }

    renderResults(schoolsOf());
  </script>
</body>
</html>
