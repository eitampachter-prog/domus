# Domus: Stitch screen prompts

Stitch project: "Domus – אב טיפוס" (`projects/11405005407106127418`), design system "Domus Cyber-Home".
Every prompt assumes Hebrew, full RTL (`dir="rtl"`), the Rubik font, and the design system's colors.
Status: ✅ = in the project, ⏳ = not created yet.

## Main flow

### 01 Onboarding ⏳
Domus app – Onboarding welcome screen. Hebrew, fully RTL (dir="rtl"). Playful illustration of three roommates in a cozy apartment with a mint "⚡ +35" badge. Logo "Domus". Headline "הבית המשותף, הוגן יותר". Body "מתעדים מטלות בתמונה, ה־AI מעריך את המאמץ, וכל אחד מקבל נקודות על התרומה שלו." Feature rows: "📸 צלמו לפני ואחרי", "🤖 הערכת מאמץ חכמה", "🏆 זירת קארמה ביתית". Button "בואו נתחיל", link "כבר יש לי חשבון – התחברות".

### 02 Sign up ⏳
Domus app – Sign up screen. Hebrew, fully RTL (dir="rtl"). Back arrow on the right. Title "יצירת חשבון", subtitle "רק כמה פרטים ואתם בפנים 🏡". Round avatar picker with camera badge. Fields with right-aligned Hebrew labels: "שם פרטי" (נועה), "אימייל" (noa@example.com, LTR), "סיסמה" (masked, eye icon). Checkbox "אני מסכים/ה לתנאי השימוש ולמדיניות הפרטיות". Primary button "המשך". Divider "או". Buttons "המשך עם Google", "המשך עם Apple". Bottom link "כבר רשומים? התחברות".

### 03 Create / Join a home ⏳
Domus app – Create or Join a Home screen. Hebrew, fully RTL (dir="rtl"). Stepper "שלב 2 מתוך 2". Title "איפה גרים? 🏠", subtitle "צרו בית חדש או הצטרפו לשותפים שלכם". Two big selectable cards: (1) "יצירת בית חדש" (selected) with house illustration, field "שם הבית: דירת הרצל 12" and type chips "דירת שותפים" (selected), "מעונות", "צוות / קבוצה". (2) "הצטרפות לבית קיים" with key icon and a 6-box invite code input "HRZ12K" (LTR). Info note "לאחר יצירת הבית תקבלו קוד הזמנה לשתף עם השותפים". Primary button "יצירת הבית".

### 04 Home Dashboard ✅ (two copies exist; keep one)

### 05 Before camera ⏳
Domus app – Create Task: Before photo camera screen. Hebrew, fully RTL (dir="rtl"). Full-bleed camera viewfinder showing a messy bathroom sink with stained tiles. Top bar: close X, title "מטלה חדשה · צילום Before", flash icon. Corner framing guides and hint chip "מסגרו את האזור שצריך טיפול". Segmented toggle "📸 צילום מצב" (selected) / "🧾 מסמך / קבלה". Bottom: gallery button "מהגלריה", big white shutter button, link "ללא תמונה – יצירה ידנית". Stepper "1 צילום · 2 ניתוח AI · 3 אישור" step 1 active.

### 06 AI scan ⏳
Domus app – AI scan in progress screen, Cyber-Home style. Hebrew, fully RTL (dir="rtl"). Dark indigo gradient background with mint glow. The bathroom Before photo in a rounded card with a glowing mint scan line, corner brackets, and detection tags "כיור", "אריחים", "אבנית". Title "ה־AI מנתח את התמונה…", subtitle "מזהה סוג מטלה, אזור ורמת מורכבות". Checklist: "✓ זיהוי אזור – חדר אמבטיה", "✓ זיהוי סוג – ניקיון", "◌ הערכת מורכבות…". Progress bar 70% filling right-to-left. Note "זו הערכה תומכת – תוכלו לבדוק ולשנות לפני הפרסום". Link "ביטול".

### 07 AI result and confirm points ⏳
Domus app – AI Result & Confirm Points screen. Hebrew, fully RTL (dir="rtl"). Header with back arrow (right), title "אישור ופרסום", stepper step 3 active. Bathroom Before photo. Card "הצעת ה־AI 🤖" with editable chips "קטגוריה: 🧽 ניקיון", "אזור: 🛁 חדר אמבטיה", complexity meter נמוכה / בינונית / גבוהה (גבוהה selected). Tags "אבנית על הברז", "כתמים על האריחים", "כיור עמוס". Title field "ניקוי יסודי של האמבטיה". Big mint points card "⚡ 35 נק׳" with −/+ stepper, caption "לפי טבלת הניקוד: ניקיון · מורכבות גבוהה. ניתן לשנות ברמה אחת", mini table "נמוכה 10 · בינונית 20 · גבוהה 35". Note "הניקוד קבוע ולא ישתנה עם הזמן". Buttons "פרסום ללוח המטלות", "שמירה כטיוטה".

### 08 Chore board ⏳
Domus app – Chore Board screen. Hebrew, fully RTL (dir="rtl"). Title "לוח מטלות", subtitle "דירת הרצל 12". Status tabs "פתוחות (2)" (active), "נלקחו (1)", "בבדיקה (1)", "הושלמו". Category chips: הכל, 🧽 ניקיון, 🛒 קניות, 🧾 חשבונות, 🔧 תחזוקה. Big bounty cards with photo, mint points pill, status chip with icon+text: 1) "ניקוי יסודי של האמבטיה" ⚡35, פורסם ע״י נועה, "🟢 פתוחה", button "לקחת משימה". 2) "קניות שבועיות בסופר" ⚡25, "🟢 פתוחה", פורסם ע״י איתי. 3) "תשלום ארנונה" ⚡20, "👤 נלקחה ע״י מאיה", disabled button. Bottom tab bar from right: בית, לוח מטלות (active), +, נקודות, פרופיל.

### 09 Task details ⏳
Domus app – Task Details screen viewed by איתי. Hebrew, fully RTL (dir="rtl"). Hero Before photo of a messy bathroom, back arrow (right). Title "ניקוי יסודי של האמבטיה", chip "🟢 פתוחה", mint pill "⚡ 35 נק׳". Info grid: "קטגוריה: 🧽 ניקיון", "אזור: 🛁 אמבטיה", "מורכבות: גבוהה", "פורסם ע״י: נועה · לפני 20 דק׳". Card "מה ה־AI זיהה" with tags. Card "איך מקבלים נקודות": "1. לוקחים את המשימה  2. מצלמים After בסיום  3. ה־AI מאמת והנקודות נזקפות". Sticky button "לקחת את המשימה ⚡ 35", small text "אפשר להחזיר ללוח בכל עת".

### 10 After photo ⏳
Domus app – Complete Task: After photo screen. Hebrew, fully RTL (dir="rtl"). Title "השלמת משימה", task "ניקוי יסודי של האמבטיה", chip "👤 בביצוע ע״י איתי", pill "⚡ 35 נק׳". Side-by-side "Before" (messy) and "After" (clean, green check, link "צילום מחדש"). Tip "צלמו מאותה זווית כמו בתמונת ה־Before לאימות מדויק יותר". Note field "הערה (לא חובה)". Toggle "🧾 במקום תמונה – העלאת קבלה / אישור תשלום". Buttons "הגשה לאימות", "החזרת המשימה ללוח".

### 11 Verification success ⏳
Domus app – Verification Success screen with confetti. Hebrew, fully RTL (dir="rtl"). Big mint badge with check and "+35". Title "כל הכבוד, איתי! 🎉", subtitle "המשימה אומתה והנקודות נזקפו לחשבונך". Chip "✅ הושלמה · אומתה ע״י AI". Before/After thumbnails, AI card "רמת ביטחון: גבוהה (92%)" with checks "✓ הכיור פנוי ונקי", "✓ האריחים ללא כתמים", "✓ אותו אזור כמו ב־Before". Points card "המאזן שלך: 95 ← 130 נק׳" with karma bar. Buttons "לזירת הקארמה", "חזרה ללוח המטלות", link "לא מסכימים עם התוצאה? ערעור".

### 12 Points ledger ⏳
Domus app – Points Ledger screen for נועה. Hebrew, fully RTL (dir="rtl"). Title "הנקודות שלי". Indigo hero: "120 נק׳", circular karma meter "רמה 7", "עוד 30 נק׳ לרמה הבאה", stats "השבוע +45 · החודש +120 · 9 משימות". Filter chips "הכל", "זיכויים", "בבדיקה". Transactions by date with icon, status chip and mint amount: "השקיית עציצים במרפסת" +15 ✅; "קניות לבית" +25 ✅; "ניקוי מטבח" 20 ⏳ ממתין לבדיקה; "תשלום ועד בית" +20 ✅; "הוצאת מחזור" +10 ✅. Note "נקודות נזקפות רק לאחר אימות, ופעם אחת לכל משימה". Tab bar with נקודות active.

### 13 Household activity ⏳
Domus app – Household Activity screen. Hebrew, fully RTL (dir="rtl"). Title "הפעילות בבית", subtitle "דירת הרצל 12 · החודש". Toggle שבוע / חודש / הכל. Donut chart: נועה 120, איתי 95, מאיה 80, center "295 נק׳ יחד". Member cards with positive titles: "נועה · 9 משימות · אלופת הסדר", "איתי · 7 משימות · מתמיד בכלים", "מאיה · 6 משימות · אלופת החשבונות". Category bars: ניקיון 55%, קניות 25%, חשבונות 20%. Banner "💚 הבית נקי יותר כשכולם תורמים — 22 משימות הושלמו החודש". No shaming language.

### 14 Profile and settings ⏳
Domus app – Profile & Household Settings. Hebrew, fully RTL (dir="rtl"). Header: avatar נועה, badge "מנהלת הבית", "120 נק׳ · רמה 7". Card "דירת הרצל 12": invite code "HRZ12K" with copy/share; members נועה, איתי, מאיה; "+ הזמנת שותף". Sections: "הבית": "טבלת ניקוד וקטגוריות", "חלוקה לצוותים / חדרים", "מי מאשר ערעורים: חבר בית אחר"; "פרטיות": "מי רואה את התמונות: חברי הבית בלבד", "שמירת תמונות: 30 יום", "מחיקת התמונות שלי"; "כללי": "התראות", "שפה: עברית", "יציאה מהבית" (coral). Tab bar with פרופיל active.

## Alternate path and system states

### 15 Verification: retake needed ⏳
Domus app – Verification result: needs another photo. Hebrew, fully RTL (dir="rtl"). Amber illustration of a blurry camera. Title "צריך עוד תמונה 📸", chip "⏳ נדרשת תמונה נוספת". Explanation "התמונה חשוכה מדי ולא ניתן להשוות לתמונת ה־Before". Before / blurry After thumbnails. Tips: "הדליקו אור", "צלמו מאותה זווית", "הכניסו את כל האזור למסגרת". Buttons "צילום מחדש", "שליחה לבדיקה אנושית".

### 16 Verification: not approved ⏳
Domus app – Verification result: not approved. Hebrew, fully RTL (dir="rtl"). Calm coral (not aggressive) icon. Title "הביצוע לא אושר הפעם", chip "✖ לא אושר" with icon. Reason card "ה־AI לא זיהה שינוי באזור הכיור – נראה שעדיין יש אבנית על הברז". Before/After side by side with a highlighted area. Buttons "השלמה והגשה חוזרת", "ערעור – שליחה לבדיקה של חבר בית", link "החזרת המשימה ללוח". Supportive note "קורה! אפשר לנסות שוב בלי לאבד את המשימה".

### 17 Review queue ⏳
Domus app – Review Queue screen. Hebrew, fully RTL (dir="rtl"). Title "ממתינות לבדיקה", subtitle "בדיקה אנושית כשה־AI לא בטוח או כשהוגש ערעור". List cards with Before/After thumbnails, mint points, reason chip: "ניקוי מטבח" · מאיה · ⚡20 · "🤔 ה־AI לא בטוח (54%)"; "ניקוי יסודי של האמבטיה" · איתי · ⚡35 · "📣 ערעור". Note "לא ניתן לבדוק משימה שביצעתם בעצמכם".

### 18 Review detail ⏳
Domus app – Review detail screen. Hebrew, fully RTL (dir="rtl"). Task "ניקוי מטבח", performed by מאיה, ⚡20. Large Before/After comparison with slider. AI card "רמת ביטחון 54% – משטח מסודר, לא ברור אם נוקה". Note from מאיה "ניקיתי גם את הכיריים". Reviewer נועה. Buttons "אישור וזיכוי 20 נק׳" (mint), "בקשת תמונה נוספת", "דחייה" (outline coral) with reason field.

### 19 Empty board ⏳
Domus app – Chore board empty state. Hebrew, fully RTL (dir="rtl"). Clean friendly illustration of a sparkling tidy living room with a small robot vacuum and a star. Title "אין כרגע מטלות פתוחות ✨", body "הבית מצוחצח! ראיתם משהו שצריך טיפול? פתחו את האתגר הראשון". Primary button "+ פתיחת מטלה חדשה". Tab bar with לוח מטלות active.

### 20 Upload failed ⏳
Domus app – Photo upload failed state. Hebrew, fully RTL (dir="rtl"). After-photo screen dimmed behind a bottom sheet: cloud-with-x icon, title "ההעלאה נכשלה", body "בדקו את החיבור לאינטרנט ונסו שוב. התמונה נשמרה במכשיר". Progress bar stopped at 62% in coral. Buttons "ניסיון חוזר", "ביטול".

### 21 Camera permission denied ⏳
Domus app – Camera permission denied state. Hebrew, fully RTL (dir="rtl"). Illustration of a camera with a lock. Title "אין גישה למצלמה", body "כדי לתעד מטלות Domus צריכה הרשאה למצלמה. אפשר לשנות זאת בהגדרות המכשיר". Buttons "פתיחת ההגדרות", "העלאה מהגלריה במקום".

### 22 Task already claimed ⏳
Domus app – Task already claimed state. Hebrew, fully RTL (dir="rtl"). Task details of "קניות שבועיות בסופר" ⚡25 in background, with a bottom sheet: avatar of מאיה, title "מאיה הקדימה אותך! 🏃‍♀️", body "המשימה נלקחה לפני רגע. יש עוד משימות פתוחות שמחכות לך", chip "👤 נלקחה ע״י מאיה". Buttons "למשימות פתוחות אחרות", "סגירה".
