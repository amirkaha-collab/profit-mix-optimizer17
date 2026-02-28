# Streamlit – מנוע תמהילי קרנות השתלמות (Embedded Data + RTL)

## מה השתנה?
- **אין העלאת קבצים למשתמש**: שני קבצי האקסל כבר כלולים בתיקיית `data/`
  - `data/קרנות השתלמות פברואר 2026.xlsx`
  - `data/ציוני שירות.xlsx`
- ההגדרות (מספר קופות / ערבוב מנהלים / צעד משקלים / דירוג ראשי) נמצאות במסך הראשי (Tab 1) ולא בסיידבר.

## מבנה תיקייה
```
app.py
requirements.txt
data/
  ├─ קרנות השתלמות פברואר 2026.xlsx
  └─ ציוני שירות.xlsx
```

## סיסמה
- ברירת מחדל: `1234`
- מומלץ ב-Streamlit Cloud להגדיר Secrets:
  - `APP_PASSWORD`

## הרצה מקומית
```bash
pip install -r requirements.txt
streamlit run app.py
```

## פריסה ל-Streamlit Cloud (בקצרה)
1. פתח Repo ב-GitHub והעלה אליו את כל התיקייה (כולל `data/`)
2. ב-Streamlit Cloud → New app → בחר את ה-Repo
3. Secrets (אופציונלי): הגדר `APP_PASSWORD`
4. Deploy
