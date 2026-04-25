# 🎯 GapHunter

**GapHunter** is a professional automation tool designed to identify businesses that lack a digital presence. By leveraging the Google Maps API (via Serper.dev), it discovers local businesses in specific sectors and locations, filters those without websites, and ranks them by their local influence (review count).

This tool is built for entrepreneurs, digital agencies, and freelancers looking to bridge the "digital gap" for local businesses.

---

## 🚀 Features

- **Automated Discovery**: Scrape hundreds of businesses in any sector and location.
- **Smart Filtering**: Automatically identifies businesses that do NOT have a website listed.
- **Lead Scoring**: Sorts potential leads by their review count to help you prioritize high-impact targets.
- **Excel Compatible Export**: Saves results into structured CSV files formatted for Microsoft Excel.
- **Technical Debt Free**: Modular architecture with logging, type hints, and robust error handling.

---

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Ali-bot-prog/GapHunter.git
cd GapHunter
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configuration

Create a `.env` file in the root directory and add your Serper.dev API key:

```env
MAPS_API_KEY=your_serper_api_key_here
```

*You can get a free API key at [serper.dev](https://serper.dev).*

---

## 📖 Usage

Run the automation with a single command:

```bash
python main.py
```

### Customization

You can change the target sector and location in `main.py`:

```python
SECTOR = "restoran"
LOCATION = "Ünye"
TARGET_COUNT = 50
```

---

## 📂 Project Structure

- `main.py`: Entry point for the automation.
- `scraper.py`: Core logic for interacting with the Serper/Google Maps API.
- `processor.py`: Data filtering, sorting, and export logic.
- `reports/`: (Auto-generated) Directory where CSV results are saved.
- `.gitignore`: Ensures sensitive files like `.env` are not pushed to GitHub.

---

## 🤝 Contributing

GapHunter geliştirilmeye açık bir projedir! Her türlü katkıya (Pull Request) ve yeni fikre açığız. Özellikle şu alanlarda yardıma ihtiyacımız var:

- 🤖 **AI Enhancements**: İşletme büyüklüğünü daha hassas ölçen yeni algoritmalar.
- 📧 **Automation**: Filtrelenen işletmelere özel teklif sunan otomatik mail modülleri.
- 🌐 **Dashboard**: Verilerin izlenebileceği basit bir web arayüzü.

### Nasıl Katkı Sağlarsınız?

1. Repoyu fork'layın.
2. Yeni bir özellik için branch oluşturun (`git checkout -b feature/AmazingFeature`).
3. Değişikliklerinizi commit edin (`git commit -m 'Add: AmazingFeature'`).
4. Branch'inizi push edin (`git push origin feature/AmazingFeature`).
5. Bir Pull Request açın.

---

## 🛡️ License & Copyright

This project is open-source. However, the implementation and logic are optimized for high-performance lead generation.

**© 2026 OmNexus. All Rights Reserved.**
