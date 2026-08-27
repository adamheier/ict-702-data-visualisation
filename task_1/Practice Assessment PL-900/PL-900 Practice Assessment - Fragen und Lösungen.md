# PL-900 Practice Assessment – Fragen und Lösungen (1. Versuch)

Diese Datei fasst alle Fragen deines ersten Versuchs im PL-900 (Microsoft Power Platform Fundamentals) Practice Assessment zusammen, so wie sie in den Screenshots im Ordner "Practice Assessment PL-900" dokumentiert sind. Fragen- und Antworttext wurden in der Originalsprache (Englisch) belassen, die Struktur-Labels sind auf Deutsch. Am Ende findest du eine Übersicht, an welchen Teilgebieten du laut Testergebnis noch arbeiten solltest.

**Gesamtergebnis des 1. Versuchs: 52 %** (Zielwert laut Test: 80 % oder höher)

---

### Frage 1
**Frage:** You plan to create a Power Apps app.

You need to enable users to read and write data from SharePoint and OneDrive for Business.

What should you use?
**Antwortmöglichkeiten:**
- A Canvas app
- A Model-driven app
- Power Pages
- A Business process flow

**Gewählte Antwort (1. Versuch):** Keine Auswahl im Screenshot erkennbar (Frage noch unbeantwortet)
**Korrekte Lösung:** A Canvas app *(Canvas Apps können sich direkt mit SharePoint und OneDrive for Business verbinden; Model-driven Apps basieren auf Dataverse, Power Pages ist für externe Websites, Business Process Flows sind keine Datenquellen-Anbindung)*
**Erklärung:** Im Screenshot nicht sichtbar (Frage wurde nicht ausgewertet gezeigt).

---

### Frage 2
**Frage:** You create an app.

You need to ensure that the app displays data from an Azure SQL database.

What should you use?
**Antwortmöglichkeiten:**
- Model-driven app
- Power Pages
- Canvas apps
- Microsoft Dataverse

**Gewählte Antwort (1. Versuch):** Model-driven app ❌ (falsch)
**Korrekte Lösung:** Canvas apps
**Erklärung:** Canvas-Apps können Daten aus verschiedenen Quellen nutzen, einschließlich Azure-SQL-Datenbanken. Model-driven Apps verwenden Daten aus Microsoft Dataverse, nicht aus Azure-SQL-Datenbanken. Microsoft Dataverse ist selbst eine Datenplattform, kein App-Typ.

---

### Frage 3
**Frage:** You have a Microsoft Power Apps canvas app named App1 that records guest check-in details at a hotel. App1 uses a Microsoft Dataverse table.

You need to design App1 to meet the following requirements:
- Collect the guest's name, meal choice, and additional preferences.
- Display a message if a guest selects a meal option that is unavailable.

What should you do?
**Antwortmöglichkeiten:**
- Add a form and fields and use the OnSubmit property to show the message.
- Add an Edit form bound to Dataverse and include the required fields. Use a formula on the meal choice control to display the message.
- Add the column that contains each guest's meal choice, rename it Guest Meal Choice, and mark the Name field as required.
- Create a new app that uses the existing Dataverse table.

**Gewählte Antwort (1. Versuch):** Add an Edit form bound to Dataverse... ✅ (richtig)
**Korrekte Lösung:** Add an Edit form bound to Dataverse and include the required fields. Use a formula on the meal choice control to display the message.
**Erklärung:** Ein Edit-Formular, gebunden an die Dataverse-Tabelle, mit einer Formel (z. B. If-Anweisung) am Mahlzeit-Steuerelement zeigt die Nachricht sofort bei Auswahl an – Echtzeit-Feedback. Eine neue App ist unnötig, das bloße Umbenennen/Pflichtsetzen einer Spalte deckt keine bedingte Nachricht ab, und OnSubmit würde die Nachricht erst nach dem Absenden zeigen.

---

### Frage 4
**Frage:** You have a Power Platform environment that contains a model-driven app named Sales App. Sales App includes a Microsoft Dataverse table named Account.

You need to create a canvas app named Account App that will use the Account table as its data source. Account App will be used by the sales team. Your solution must minimize configuration effort.

What should you do in the Power Apps maker portal?
**Antwortmöglichkeiten:**
- Create a blank canvas app, connect it to the Account table, and save it.
- Create a blank model-driven app and add the Account table.
- Create an app based on a template and replace the data source with the Account table.
- Open Sales App and add a new canvas page for Account App.

**Gewählte Antwort (1. Versuch):** Create an app based on a template... (Auswertung im Screenshot nicht farblich markiert)
**Korrekte Lösung:** Im Screenshot nicht eindeutig ersichtlich – nach PL-900-Logik ist "Create a blank canvas app, connect it to the Account table, and save it" der Standardweg mit minimalem Konfigurationsaufwand für eine reine Datenanbindung.
**Erklärung:** Im Screenshot keine Auswertung sichtbar.

---

### Frage 5
**Frage:** You create a canvas app. You add a label control to your screen.

You need to set the text color to red.

What are three possible ways to achieve this goal? Each correct answer presents a complete solution.
**Antwortmöglichkeiten:**
- Select the label control. Select the color picker control in the toolbar and choose red from the color menu.
- Select the label control. Choose the Fill property in the formula bar. Set the formula value to Color.Red.
- Select the label control. Choose the Color property in the formula bar. Set the formula value to Color.Red.
- Select the label control. Open the Properties pane and choose the Advanced tab. Find the Fill property and add Color.Red to the textbox.
- Select the label control. Open the Properties pane and choose the Advanced tab. Find the Color property and add Color.Red to the textbox.

**Gewählte Antwort (1. Versuch):** Color picker ✅, Fill-Formel ❌ (falsch gewählt), Color-Formel ✅ — die korrekte "Advanced tab → Color property" wurde nicht ausgewählt → teilweise falsch
**Korrekte Lösung:** Color picker in der Toolbar + Color-Eigenschaft in der Formelleiste + Color-Eigenschaft im Advanced-Tab (alle drei setzen **Color**, nicht Fill)
**Erklärung:** **Fill** legt die Hintergrundfarbe fest, nicht die Textfarbe – nur **Color** steuert die Textfarbe, egal ob über Color Picker, Formelleiste oder Advanced-Tab gesetzt.

---

### Frage 6
**Frage:** You create and publish a canvas app.

Users report issues with the latest version of the app.

You need to revert the app to an earlier working version.

Which two actions should you perform? Each correct answer presents part of the solution.
**Antwortmöglichkeiten:**
- Edit the app, undo all the changes, and publish the app.
- Select an earlier version of the app and click on Restore.
- Publish the restored version of the app.
- Export the previous version of the app and import it.

**Gewählte Antwort (1. Versuch):** "Select an earlier version... Restore" ✅ + "Publish the restored version" ✅ (richtig)
**Korrekte Lösung:** Select an earlier version of the app and click on Restore. + Publish the restored version of the app.
**Erklärung:** Über die Versionierung kann eine frühere Version wiederhergestellt (Restore) werden; diese wiederhergestellte Version muss anschließend veröffentlicht werden. Ein manuelles Rückgängigmachen von Änderungen oder ein Export/Import ist dafür nicht nötig bzw. nicht möglich (Export liefert immer die neueste Version).

---

### Frage 7
**Frage:** You create a canvas app that is connected to a Microsoft Dataverse table.

You need to share the app.

Which two actions should you perform? Each correct answer presents part of the solution.
**Antwortmöglichkeiten:**
- Notify the users by email.
- Allow the users to edit the app.
- Publish the app.
- Assign a security role.

**Gewählte Antwort (1. Versuch):** Publish the app. + Assign a security role. ✅ (richtig)
**Korrekte Lösung:** Publish the app. + Assign a security role.
**Erklärung:** Eine Canvas-App muss veröffentlicht sein, bevor sie geteilt werden kann; ist sie mit Dataverse verbunden, muss zusätzlich eine Security Role zugewiesen werden. Eine E-Mail-Benachrichtigung ist nur informativ, Bearbeitungsrechte sind für das Teilen nicht erforderlich.

---

### Frage 8
**Frage:** You configure a canvas app to track and order office stationery. The app allows users to order multiple stationery items.

The items selected by the user must be reset each time a user reopens the app.

You need to store user selections.

What should you use?
**Antwortmöglichkeiten:**
- A Collection
- Dataverse
- SharePoint
- A Variable

**Gewählte Antwort (1. Versuch):** Dataverse ❌ (falsch)
**Korrekte Lösung:** A Collection
**Erklärung:** Eine Collection speichert Daten nur temporär innerhalb der App-Sitzung und geht beim erneuten Öffnen verloren – genau das ist gefordert. Dataverse/SharePoint würden die Auswahl dauerhaft speichern, eine Variable kann nur einen einzelnen Wert, nicht mehrere Items speichern.

---

### Frage 9
**Frage:** You plan to create a canvas app that allows users to view a list of current scores for all local professional sporting events.

Each game should display the following:
- Name of the game.
- Amount of time left in the game.
- A link to a map of the game's location.

You need to add controls to your Power Apps app.

Which two controls should you use? Each correct answer presents part of the solution.
**Antwortmöglichkeiten:**
- Form
- Screen
- List box
- Data table
- Gallery

**Gewählte Antwort (1. Versuch):** Form ❌ + Screen ✅ (teilweise falsch, Gallery fehlte)
**Korrekte Lösung:** Screen + Gallery
**Erklärung:** Jede Canvas-App braucht mindestens einen Screen als Container. Eine Gallery zeigt mehrere Datensätze (hier: Spiele) mit beliebigen Steuerelementen pro Eintrag (z. B. einem Link zum Standort). Ein Form-Steuerelement zeigt nur einen Datensatz, List Box dient der Werteauswahl, Data Table erlaubt keine reichhaltige Formatierung wie Hyperlinks.

---

### Frage 10
**Frage:** You use a Microsoft Dataverse table to store products. You create a canvas app to list the products in the app.

You need to enable users to view the product code, description, and image of each product.

Which control should you use?
**Antwortmöglichkeiten:**
- Gallery
- Form
- Drop-down
- Data table

**Gewählte Antwort (1. Versuch):** Data table ❌ (falsch)
**Korrekte Lösung:** Gallery
**Erklärung:** Die Gallery zeigt mehrere Datensätze inklusive verschiedener Datentypen wie Bilder an. Form zeigt nur einen Datensatz, Drop-down und Data Table können keine Bildspalten aus Dataverse darstellen.

---

### Frage 11
**Frage:** A company uses Microsoft Power Platform.

You need to identify the features of model-driven apps.

What are three features of model-driven apps? Each correct answer presents a complete solution.
**Antwortmöglichkeiten:**
- They adjust the layout of the UI automatically in response to changes in a device's orientation or screen resolution.
- They connect to multiple data sources.
- They control navigation between forms by using Microsoft Power Fx formulas.
- They embed Power BI dashboards.
- They guide users by using business process flows.

**Gewählte Antwort (1. Versuch):** UI-Anpassung ✅ + mehrere Datenquellen ❌ + Power-BI-Dashboards ✅ (teilweise falsch, "guide users by BPF" fehlte)
**Korrekte Lösung:** UI passt sich automatisch an + Power-BI-Dashboards einbetten + Nutzer werden durch Business Process Flows geführt
**Erklärung:** Model-driven Apps basieren auf einer einzigen Datenquelle (Dataverse), nicht auf mehreren. Ihr vordefiniertes UI-Modell passt sich automatisch an Bildschirmgröße/Ausrichtung an, sie können Power-BI-Dashboards und Business Process Flows als Komponenten einbinden. Navigation erfolgt über das Datenmodell, nicht über Power-Fx-Formeln.

---

### Frage 12
**Frage:** A company uses Microsoft Dataverse.

You need to define views to display data in model-driven apps.

Which three items can you configure in the view designer? Each correct answer presents part of the solution.
**Antwortmöglichkeiten:**
- The apps in which the view is available.
- The columns included in the view.
- The filter for rows shown in the view.
- The sort order of rows in the view.
- Whether the user can filter the contents of the view in the app.

**Gewählte Antwort (1. Versuch):** Spalten ✅ + Filter für Zeilen ✅ + Sortierung ✅ (richtig)
**Korrekte Lösung:** Spalten der View + Filter für angezeigte Zeilen + Sortierreihenfolge
**Erklärung:** Der View-Designer legt Spalten, Filterkriterien und Sortierung fest. Welche Apps eine View nutzen, wird im App-Designer bestimmt, und alle Views können vom Nutzer in der App ohnehin gefiltert werden.

---

### Frage 13
**Frage:** A company uses a model-driven app for customer data management.

You create a new column.

Users report that they cannot view the column when they edit records.

You need to ensure users can view the column.

Which two actions should you perform? Each correct answer presents part of the solution.
**Antwortmöglichkeiten:**
- Add the column to the view.
- Add the column on the form.
- Publish customizations.
- Add a page.

**Gewählte Antwort (1. Versuch):** Spalte zur View hinzufügen ❌ + Customizations veröffentlichen ✅ (teilweise falsch, "Add the column on the form" fehlte)
**Korrekte Lösung:** Add the column on the form. + Publish customizations.
**Erklärung:** Formulare (Forms) steuern, welche Spalten beim Bearbeiten eines Datensatzes sichtbar sind – eine neue Spalte wird dort nicht automatisch angezeigt. Sie muss dem Form hinzugefügt und die Änderung veröffentlicht werden. Views betreffen nur die Listendarstellung, nicht die Bearbeitungsansicht.

---

### Frage 14
**Frage:** You have a model-driven app that contains the following components:
- Microsoft Dataverse tables
- A business process flow
- Model-driven forms

You need to identify what each component represents.

What should you identify?
**Antwortmöglichkeiten:**
- Dataverse tables are data components, model-driven forms are UI components, and a business process flow is a logic component.
- Dataverse tables are logic components, model-driven forms are data components, and a business process flow is a UI component.
- Dataverse tables are logic components, model-driven forms are UI components, and a business process flow is a data component.
- Dataverse tables are UI components, model-driven forms are data components, and a business process flow is a logic component.

**Gewählte Antwort (1. Versuch):** Dataverse tables = data, forms = UI, business process flow = logic ✅ (richtig)
**Korrekte Lösung:** Dataverse tables are data components, model-driven forms are UI components, and a business process flow is a logic component.
**Erklärung:** Dataverse-Tabellen bilden die Datenschicht, Formulare die UI-Schicht (Anzeige/Interaktion), Business Process Flows die Logikschicht (Prozessregeln und -führung).

---

### Frage 15
**Frage:** You plan to create Power Pages websites on a new Microsoft Power Platform environment.

You need to accelerate the creation of the websites.

Which two types of templates can you use to meet the requirement? Each answer presents a complete solution.
**Antwortmöglichkeiten:**
- Blank page
- Dynamics 365
- Solution
- Starter

**Gewählte Antwort (1. Versuch):** Dynamics 365 ❌ + Starter ✅ (teilweise falsch)
**Korrekte Lösung:** Solution + Starter
**Erklärung:** Solution-Vorlagen sind vollständige, fertige Websites für gängige Szenarien; Starter-Vorlagen liefern vorgefertigte Seiten mit Layout/Farben. Blank Page erstellt nur eine leere Startseite, Dynamics-365-Vorlagen setzen eine installierte D365-App voraus.

---

### Frage 16
**Frage:** The manager of a retail store wants to provide a self-service solution for customers who want to track their orders.

You need to recommend a solution based on Microsoft Power Platform.

Which solution should you recommend?
**Antwortmöglichkeiten:**
- model-driven app using Power Apps
- canvas app using Power Apps
- website portal using Power Pages
- dashboard using Power BI

**Gewählte Antwort (1. Versuch):** website portal using Power Pages ✅ (richtig)
**Korrekte Lösung:** website portal using Power Pages
**Erklärung:** Power Pages richtet sich an externe Benutzer (hier: Kunden). Canvas-/Model-driven Apps sind für interne Nutzer, Power BI dient der Analyse, nicht der transaktionalen Selbstbedienung.

---

### Frage 17
**Frage:** You have a Power Platform environment.

You need to create a Microsoft Power Pages site in the environment and add a Microsoft Dataverse table that can be used within the site.

What should you use?
**Antwortmöglichkeiten:**
- Microsoft Power Apps Studio
- Microsoft Power Automate
- Power Pages design studio
- the Power Platform admin center

**Gewählte Antwort (1. Versuch):** Power Pages design studio ✅ (richtig)
**Korrekte Lösung:** Power Pages design studio
**Erklärung:** Das Power Pages Design Studio dient dem Erstellen/Anpassen von Power-Pages-Websites inkl. Dataverse-Tabellenanbindung. Power Apps Studio ist für Canvas-/Model-driven Apps, Power Automate für Flows, das Admin Center für Umgebungsverwaltung.

---

### Frage 18
**Frage:** You have a Power Platform environment.

A solution in the environment contains a Microsoft Power Pages site.

You plan to deploy the solution to a downstream environment.

You need to ensure that the Power Pages site is available and fully functional in the downstream environment.

What should you do?
**Antwortmöglichkeiten:**
- From Microsoft Power Apps, publish the site.
- From Microsoft Power Apps, run the Import solution wizard.
- From the Power Platform admin center, create a new site that uses data from the Dataverse database.
- From the Power Platform admin center, select the site and select Configure.

**Gewählte Antwort (1. Versuch):** From the Power Platform admin center, select the site and select Configure. ✅ (richtig)
**Korrekte Lösung:** From the Power Platform admin center, select the site and select Configure.
**Erklärung:** Nach dem Import einer Lösung mit Power-Pages-Site muss die Site im Admin Center explizit über "Configure" aktiviert werden, bevor sie funktioniert. Bloßes Veröffentlichen oder Neuanlegen reicht nicht aus.

---

### Frage 19
**Frage:** You have a Power Platform environment.

You plan to create a Microsoft Dataverse table named Project.

You need to ensure that users can perform the following tasks:
- Create project records.
- Enter project information simultaneously from multiple devices.
- Associate project records with a Microsoft Teams channel.
- Access project records from a Teams channel.
- Use Microsoft Excel to modify project records.

What should you use to create the table?
**Antwortmöglichkeiten:**
- Microsoft Copilot Studio
- Microsoft Power Apps
- Microsoft Power BI
- Microsoft Power Pages

**Gewählte Antwort (1. Versuch):** Microsoft Power Apps ✅ (richtig)
**Korrekte Lösung:** Microsoft Power Apps
**Erklärung:** Dataverse-Tabellen werden über Power Apps erstellt/verwaltet, das eine vollständige Integration mit Teams, Excel und weiteren Microsoft-365-Diensten bietet. Power Pages ist für externe Websites, Power BI für Analysen, Copilot Studio für Chatbots gedacht.

---

### Frage 20
**Frage:** You have a Microsoft Dataverse environment that contains a solution. The solution contains a Microsoft Power Pages site.

You need to move the Power Pages site to another environment.

What should you do?
**Antwortmöglichkeiten:**
- Create a new Power Pages site in the other environment. Create a solution and add the new site to the solution.
- Create a new solution in the other environment. Add the Power Pages site to the solution.
- Export the Power Pages site, create a new Power Pages site in the other environment, and then import the exported site.
- Export the solution, and then import the solution into the other environment.

**Gewählte Antwort (1. Versuch):** Export the Power Pages site, create a new site, import the exported site. ❌ (falsch)
**Korrekte Lösung:** Export the solution, and then import the solution into the other environment.
**Erklärung:** Eine Power-Pages-Site wird über den Export/Import der zugehörigen **Lösung** zwischen Umgebungen verschoben – das erhält die Konfiguration. Ein direkter Export/Import der Site (ohne Lösung) wird nicht unterstützt.

---

### Frage 21
**Frage:** You have a Microsoft Power Pages site that uses Microsoft Dataverse for data storage.

You plan to implement a custom page template that will display data from Dataverse.

You need to extend the site by using the custom page template.

What should you use?
**Antwortmöglichkeiten:**
- HTML, CSS, and Liquid
- JavaScript
- the Power Pages Web API
- the Power Platform command line interface (CLI)

**Gewählte Antwort (1. Versuch):** the Power Pages Web API ❌ (falsch)
**Korrekte Lösung:** HTML, CSS, and Liquid
**Erklärung:** Benutzerdefinierte Seitenvorlagen werden mit HTML, CSS und Liquid erstellt; Liquid bindet Dataverse-Daten serverseitig ein. Die Web API dient clientseitigen CRUD-Operationen, JavaScript nur der Interaktivität, die CLI der Administration/Bereitstellung.

---

### Frage 22
**Frage:** A sales company plans to use Microsoft Power Platform and Dataverse to build solutions to help manage its day-to-day operations.

The company requires a solution that at the end of each workday automatically identifies and cancels appointments from the previous workday that are not marked as complete.

You need to create a Power Automate cloud flow that meets the requirement.

Which trigger type should you create?
**Antwortmöglichkeiten:**
- automatic flow that is triggered when an appointment is updated
- scheduled flow that runs daily at a specific time
- instant flow triggered when someone selects a button
- automatic flow that is triggered when a new appointment is created

**Gewählte Antwort (1. Versuch):** scheduled flow that runs daily at a specific time ✅ (richtig)
**Korrekte Lösung:** scheduled flow that runs daily at a specific time
**Erklärung:** Scheduled Flows laufen nach festem Zeitplan und können dabei mehrere Datensätze gleichzeitig bearbeiten – genau das ist hier gefragt. Ereignisbasierte oder manuelle Trigger passen nicht zu einer täglich wiederkehrenden Massenaktion.

---

### Frage 23
**Frage:** You are building a desktop flow by using Microsoft Power Automate for desktop. The desktop flow must run when triggered by a button in a cloud flow.

You need to create the desktop flow and ensure that it can be triggered from the cloud flow.

What should you do?
**Antwortmöglichkeiten:**
- Create a desktop flow and ensure that the machine where the flow runs is registered in Power Automate.
- Create a desktop flow and run it from Power Automate.
- Create a desktop flow and run it from Windows Task Scheduler.
- Create a desktop flow, and then connect it to the cloud flow by using an on-premises data gateway.

**Gewählte Antwort (1. Versuch):** Create a desktop flow and run it from Power Automate. ❌ (falsch)
**Korrekte Lösung:** Create a desktop flow and ensure that the machine where the flow runs is registered in Power Automate.
**Erklärung:** Damit ein Cloud-Flow einen Desktop-Flow auslösen kann, muss der ausführende Computer in Power Automate registriert und online sein. Task Scheduler ist nicht integriert, das On-Premises-Gateway dient nur der Datenanbindung, nicht dem Auslösen von Desktop-Flows.

---

### Frage 24
**Frage:** You have a Microsoft Power Apps app that uses a Microsoft Dataverse database.

When a user presses a button in the app, the solution must create a record in a Microsoft SharePoint Online list and a record in the Dataverse database. Both operations must run in parallel.

You need to design a solution that supports parallel branches.

What should you use?
**Antwortmöglichkeiten:**
- a business process flow
- a business rule
- a cloud flow
- a desktop flow

**Gewählte Antwort (1. Versuch):** a cloud flow ✅ (richtig)
**Korrekte Lösung:** a cloud flow
**Erklärung:** Cloud Flows unterstützen Verzweigungen und parallele Ausführung. Business Process Flows führen Nutzer durch Prozessphasen, Desktop Flows automatisieren lokale Aufgaben, Business Rules wirken nur innerhalb einer Dataverse-Tabelle – keines davon kann Aktionen dienstübergreifend parallel orchestrieren.

---

### Frage 25
**Frage:** You have a Microsoft Power Automate cloud flow.

You need to create another flow that uses the same connectors as the first flow. The solution must minimize development effort.

Which type of flow should you create?
**Antwortmöglichkeiten:**
- a cloud flow from a connector
- a cloud flow from a solution
- a cloud flow from a template
- a cloud flow from blank

**Gewählte Antwort (1. Versuch):** a cloud flow from a solution ❌ (falsch)
**Korrekte Lösung:** a cloud flow from a template
**Erklärung:** Vorlagen (Templates) enthalten bereits vorkonfigurierte Trigger, Aktionen und Connectors, was den Entwicklungsaufwand minimiert. Ein leerer Flow oder ein Flow aus einem einzelnen Connector erfordert mehr manuelle Konfiguration; eine Solution übernimmt Connectors nicht automatisch.

---

### Frage 26
**Frage:** You need to build a workflow that sends an email each time a new item is added to a SharePoint Online list.

Which two components should you use? Each correct answer presents part of the solution.
**Antwortmöglichkeiten:**
- Power Apps
- Power Automate
- Power BI
- Microsoft Copilot Studio
- Connectors

**Gewählte Antwort (1. Versuch):** Power Automate + Connectors ✅ (richtig)
**Korrekte Lösung:** Power Automate + Connectors
**Erklärung:** Ein Cloud-Flow mit SharePoint-Online-Connector (Trigger) und einem E-Mail-Connector (Aktion) erfüllt die Anforderung. Power Apps liefert nur UI, Power BI dient der Visualisierung, Copilot Studio der Bot-Interaktion – keines davon wird hier benötigt.

---

### Frage 27
**Frage:** A company uses a Microsoft Copilot Studio copilot to manage routine customer requests. You use Power Automate to pass these requests to your back-end systems.

You need to mimic the onscreen actions that customer service agents perform manually.

What should you use?
**Antwortmöglichkeiten:**
- Connector
- cloud flow
- desktop flow
- business process flow

**Gewählte Antwort (1. Versuch):** cloud flow ❌ (falsch)
**Korrekte Lösung:** desktop flow
**Erklärung:** Desktop Flows führen Aktionen auf älteren Anwendungen ohne API aus, indem sie Bildschirmaktionen (Tastatur/Maus) nachahmen. Cloud Flows arbeiten dagegen über API-Aufrufe und ahmen keine Bildschirminteraktionen nach.

---

### Frage 28
**Frage:** A company receives documents as PDF attachments by email.

You need to process these documents automatically without user interaction by using Microsoft Power Platform.

Which two components should you use? Each correct answer presents part of the solution.
**Antwortmöglichkeiten:**
- AI Builder
- Canvas app
- Power Automate cloud flow
- Power BI
- Copilot Studio

**Gewählte Antwort (1. Versuch):** Power Automate cloud flow ✅ + Copilot Studio ❌ (teilweise falsch)
**Korrekte Lösung:** AI Builder + Power Automate cloud flow
**Erklärung:** Das AI-Builder-Dokumentverarbeitungsmodell extrahiert Informationen aus Dokumenten und wird aus einem per E-Mail-Eingang getriggerten Cloud-Flow aufgerufen. Canvas Apps, Power BI und Copilot Studio erfordern Benutzerinteraktion bzw. dienen anderen Zwecken (Visualisierung, Chatbot) und passen nicht zu "ohne Benutzerinteraktion".

---

### Frage 29
**Frage:** You plan to create a flow using Power Automate. The flow will allow users to press a button in the Power Automate mobile app, which will send a reminder email notification.

You need to determine which type of flow to create.

Which type of flow should you create?
**Antwortmöglichkeiten:**
- Scheduled
- Automated
- Business process
- Instant

**Gewählte Antwort (1. Versuch):** Instant ✅ (richtig)
**Korrekte Lösung:** Instant
**Erklärung:** Instant Flows werden manuell per Button (z. B. in der mobilen App) ausgelöst. Scheduled läuft nach Zeitplan, Automated wird durch ein Ereignis in einem anderen System getriggert, Business Process Flows führen Nutzer durch Prozessschritte – keines davon passt zu einem manuellen Button-Trigger ohne festen Zeitplan.

---

### Frage 30
**Frage:** A company has a list of new employees.

The company wants to use Teams to send a daily welcome message to new employees.

You need to write a flow that checks the list for new employees without human intervention.

Which type of flow should you use?
**Antwortmöglichkeiten:**
- Instant cloud flow
- Automated cloud flow
- Business process flow
- Scheduled cloud flow

**Gewählte Antwort (1. Versuch):** Automated cloud flow ❌ (falsch)
**Korrekte Lösung:** Scheduled cloud flow
**Erklärung:** Ein Scheduled Flow läuft täglich zu einem festen Zeitpunkt – ohne menschliches Eingreifen. Instant erfordert eine manuelle Aktion, Automated wird durch ein Ereignis (nicht durch Zeit) ausgelöst, Business Process Flows führen Menschen durch Prozesse.

---

### Frage 31
**Frage:** A company plans to create an app by using Microsoft Power Platform.

The app should be able to email sales quotes to customers.

You need to automate the process of sending sales quotes.

What should you use?
**Antwortmöglichkeiten:**
- Power Apps
- Power Automate
- Power BI
- Microsoft Copilot Studio

**Gewählte Antwort (1. Versuch):** Power Automate ✅ (richtig)
**Korrekte Lösung:** Power Automate
**Erklärung:** Power Automate kann automatisiert E-Mails mit Anhängen versenden. Power Apps liefert UI, Power BI dient Analysen, Copilot Studio dem Bot-Bau – keines davon automatisiert E-Mail-Versand.

---

### Frage 32
**Frage:** You need to build a low-code application that includes online forms for collecting and displaying information from users.

What should you use?
**Antwortmöglichkeiten:**
- Power Automate
- Power BI
- Microsoft Copilot Studio
- Power Apps

**Gewählte Antwort (1. Versuch):** Power Apps ✅ (richtig)
**Korrekte Lösung:** Power Apps
**Erklärung:** Power Apps erstellt Low-Code-Formulare/Anwendungen. Power Automate baut Workflows, Power BI Dashboards/Reports, Copilot Studio Chatbots – keines davon ist für Online-Formulare gedacht.

---

### Frage 33
**Frage:** A company plans to use Microsoft Power Platform to transform its business.

The company wants to digitize its invoice approval process to remove all manual steps.

You need to recommend the appropriate Microsoft Power Platform product.

Which product should you recommend?
**Antwortmöglichkeiten:**
- Power Apps
- Power Automate
- Power BI
- Power Pages

**Gewählte Antwort (1. Versuch):** Power Automate ✅ (richtig)
**Korrekte Lösung:** Power Automate
**Erklärung:** Power Automate dient dem Bau automatisierter Workflows/Prozesse (inkl. RPA). Power Apps erstellt Business-Apps, Power BI dient Analysen, Power Pages externen Websites.

---

### Frage 34
**Frage:** A company uses Microsoft Dynamics 365 Sales to manage its sales process.

Sales managers need access to more detailed analytics than what is available in Sales.

You need to identify which Microsoft Power Platform application creates the required analytics reports.

Which application should you select?
**Antwortmöglichkeiten:**
- Microsoft Copilot Studio
- Power Automate
- Power BI
- Power Pages

**Gewählte Antwort (1. Versuch):** Power BI ✅ (richtig)
**Korrekte Lösung:** Power BI
**Erklärung:** Power BI erstellt leistungsstarke Analysen, die u. a. in Dynamics 365 Sales konsumiert werden können. Copilot Studio erstellt Bots, Power Automate Automatisierungen, Power Pages externe Websites.

---

### Frage 35
**Frage:** A company uses Dynamics 365 Field Service to support their customers.

You need to allow external users to create a new support request.

Which Microsoft Power Platform component should you use?
**Antwortmöglichkeiten:**
- Model-driven app
- Power BI
- Power Pages
- Power Automate

**Gewählte Antwort (1. Versuch):** Power Pages ✅ (richtig)
**Korrekte Lösung:** Power Pages
**Erklärung:** Power Pages ist für den Zugriff externer Nutzer konzipiert. Model-driven Apps stehen externen Nutzern nicht zur Verfügung, Power BI dient Analysen, Power Automate löst keine Anfragen externer Nutzer aus.

---

### Frage 36
**Frage:** A company uses Microsoft Power Platform. The company builds Power Apps canvas apps, Power BI dashboards, and Microsoft Copilot Studio.

You need to identify the Microsoft Power Platform component that can be used directly with these three components.

What should you identify?
**Antwortmöglichkeiten:**
- AI Builder
- Model-driven apps
- Power Automate
- Microsoft Dataverse

**Gewählte Antwort (1. Versuch):** Power Automate ✅ (richtig)
**Korrekte Lösung:** Power Automate
**Erklärung:** Power Automate lässt sich direkt mit Canvas Apps (Flow-Trigger aus der App), Power-BI-Datenwarnungen und Copilot-Studio-Bots (Flows als Aktionen) verknüpfen.

---

### Frage 37
**Frage:** A company has a Power Pages.

You need to send a notification each week by using a third-party service. The notification must contain a summary of the records created inside the Power Pages.

Which Microsoft Power Platform component should you use?
**Antwortmöglichkeiten:**
- Power Automate
- Power BI
- Microsoft Copilot Studio
- Microsoft Dataverse

**Gewählte Antwort (1. Versuch):** Power Automate ✅ (richtig)
**Korrekte Lösung:** Power Automate
**Erklärung:** Power Automate kann über Standard- oder Custom-Connectors Drittanbieterdienste anbinden und zeitgesteuert Zusammenfassungen versenden. Power BI ist ein Analysedienst, Copilot Studio erstellt Chatbots, Dataverse ist nur die Datenplattform.

---

### Frage 38
**Frage:** You have a Power Platform environment that contains the following Microsoft Dataverse tables:
- Account: Standard table, part of a managed solution
- Product: Custom table, part of an unmanaged solution
- Sales Order: Custom table, part of a managed solution

You need to implement a new table named Invoice. The solution must meet the following requirements:
- Invoice must be associated with a standard table.
- Invoice must be associated with an existing custom table.
- Administrative effort must be minimized.

Which tables can you associate with Invoice?
**Antwortmöglichkeiten:**
- Account and Sales Order only
- Account only
- Account, Product, and Sales Order
- Product and Sales Order only

**Gewählte Antwort (1. Versuch):** Account, Product, and Sales Order ✅ (richtig)
**Korrekte Lösung:** Account, Product, and Sales Order
**Erklärung:** Es gibt keine Einschränkung, die eine Verknüpfung mit sowohl gemanagten als auch ungemanagten Custom-Tabellen verhindert. Die Einbeziehung aller drei Tabellen erfüllt beide Anforderungen (Standard- + Custom-Tabelle) mit minimalem Aufwand.

---

### Frage 39
**Frage:** You are a business user who needs to guide other users through the stages and steps of a business process by using Microsoft Dataverse.

You need to create a business process flow.

What should you use?
**Antwortmöglichkeiten:**
- Microsoft Copilot Studio
- Microsoft Power Apps
- Microsoft Power Automate
- Microsoft Power BI

**Gewählte Antwort (1. Versuch):** Microsoft Power Apps ❌ (falsch)
**Korrekte Lösung:** Microsoft Power Automate
**Erklärung:** Business Process Flows werden in Power Automate erstellt, konfiguriert und veröffentlicht und sind an Dataverse-Tabellen gebunden. Power Apps dient der App-Entwicklung, Power BI Analysen, Copilot Studio dem Bot-Bau.

---

### Frage 40
**Frage:** You are evaluating Microsoft Power Automate.

You have a desktop computer that runs Windows 11 and a laptop that runs Windows 11.

The desktop computer is in your office and is powered on from 07:00 to 17:00 each day. The laptop is used only when you work remotely. Both devices are connected to the internet.

You need to ensure that you can create workflows that automate tasks on the desktop computer, even when the laptop is turned off.

What should you do?
**Antwortmöglichkeiten:**
- Install and configure the on-premises data gateway on both computers.
- Install Microsoft Entra application proxy on both computers.
- Install Microsoft Entra application proxy on the desktop computer only.
- Install Power Automate desktop on the desktop computer and register the computer in Power Automate.

**Gewählte Antwort (1. Versuch):** Install Power Automate desktop on the desktop computer and register the computer in Power Automate. ✅ (richtig)
**Korrekte Lösung:** Install Power Automate desktop on the desktop computer and register the computer in Power Automate.
**Erklärung:** So können Desktop-Flows auf diesem Rechner laufen, sobald er eingeschaltet und online ist – unabhängig vom Laptop. Das On-Premises-Gateway dient dem Datenzugriff, nicht dem Auslösen von Desktop-Flows; Entra Application Proxy dient dem sicheren Veröffentlichen interner Apps.

---

### Frage 41
**Frage:** You use Microsoft Dataverse to develop a data model for a company.

You plan to use a custom table named **Problem** to store information about problems reported by customers. Problems will be assigned a low, medium, or high severity.

You need to capture the problem severity.

Which type of column should you use?
**Antwortmöglichkeiten:**
- Choices
- Choice
- Yes/No
- Unique number

**Gewählte Antwort (1. Versuch):** Choices ❌ (falsch)
**Korrekte Lösung:** Choice
**Erklärung:** **Choice** erlaubt genau einen Wert aus der Liste – passend für "low/medium/high". **Choices** (Mehrzahl) erlaubt Mehrfachauswahl, Yes/No nur zwei Werte, Unique Number ist ein Textfeld für eindeutige IDs.

---

### Frage 42
**Frage:** A company uses Microsoft Dataverse.

You plan to create a one-to-many relationship between two tables named **TableA** and **TableB** in Microsoft Dataverse.

You need to identify the column data type that is created for the relationship in TableB.

What should you identify?
**Antwortmöglichkeiten:**
- Alternate key
- Customer
- Lookup
- Primary key

**Gewählte Antwort (1. Versuch):** Alternate key ❌ (falsch)
**Korrekte Lösung:** Lookup
**Erklärung:** Bei einer 1:n-Beziehung entsteht auf der "Viele"-Seite (TableB) eine **Lookup**-Spalte, die den übergeordneten Datensatz referenziert (Fremdschlüssel). Alternate Keys dienen Systemintegrationen, Customer ist ein spezieller Lookup-Typ für Account/Contact, der Primary Key entsteht automatisch bei Tabellenerstellung.

---

### Frage 43
**Frage:** You have a Microsoft Dataverse environment.

You create a business process flow for a table. The business process flow has three stages.

You also create a business rule that must run whenever the value of a status column changes. The business rule must run after each stage of the business process flow is complete.

You need to ensure the business rule is active and will run as designed.

What should you do?
**Antwortmöglichkeiten:**
- In the business process flow, activate the business rule.
- In the business process flow, add the business rule as a step.
- On the table, activate the business process flow.
- On the table, activate the business rule.

**Gewählte Antwort (1. Versuch):** In the business process flow, activate the business rule. ❌ (falsch)
**Korrekte Lösung:** On the table, activate the business rule.
**Erklärung:** Business Rules werden immer auf **Tabellenebene** definiert und aktiviert, nicht innerhalb eines Business Process Flow. Eine Aktivierung "im BPF" ist nicht möglich; das Aktivieren des BPF selbst hat keinen Einfluss darauf, ob die Business Rule läuft.

---

### Frage 44
**Frage:** You have a Power Platform environment that contains a Microsoft Dataverse database.

A user named User1 plans to create a canvas app named App1 that connects to the Dataverse database. User1 will share App1 with other users.

You need to ensure that User1 can share App1. The solution must follow the principle of least privilege.

Which security role should you assign to User1?
**Antwortmöglichkeiten:**
- Delegated Admin
- Environment Maker
- System Administrator
- System Customizer

**Gewählte Antwort (1. Versuch):** Delegated Admin ❌ (falsch)
**Korrekte Lösung:** Environment Maker
**Erklärung:** **Environment Maker** ist die Rolle mit den geringsten Rechten, die Apps/Flows/Verbindungen erstellen und mit anderen teilen darf. System Customizer/Administrator sind zu weitreichend (verletzen "least privilege"), Delegated Admin betrifft von Partnern verwaltete Umgebungen.

---

### Frage 45
**Frage:** You configure security and compliance features in Microsoft Power Platform.

You need to restrict access to all social media connectors.

What should you configure?
**Antwortmöglichkeiten:**
- Microsoft Dataverse security role
- License
- Data loss prevention (DLP) policy
- Office 365 security group

**Gewählte Antwort (1. Versuch):** Office 365 security group ❌ (falsch)
**Korrekte Lösung:** Data loss prevention (DLP) policy
**Erklärung:** DLP-Richtlinien klassifizieren Connectors als Business/Non-Business/Blocked und steuern so den Zugriff auf bestimmte Connector-Kategorien wie Social Media. Security Roles regeln Tabellen-/Datensatzzugriff, Lizenzen den Produktzugriff, Security Groups den Umgebungszugriff – keines davon steuert einzelne Connectors.

---

### Frage 46
**Frage:** You plan to build a Power Apps app to meet the following requirements:
- App must be developed and tested in a non-production environment.
- App makers must be able to share the app with any user in the tenant.
- App will be updated twice a year.
- Ability to restore the environment from a backup.

You need to determine which type of Microsoft Power Platform environment to use for the app.

What should you use?
**Antwortmöglichkeiten:**
- Sandbox
- Trial
- Microsoft Dataverse for Teams
- Default

**Gewählte Antwort (1. Versuch):** Sandbox ✅ (richtig)
**Korrekte Lösung:** Sandbox
**Erklärung:** Eine Sandbox-Umgebung dient Entwicklung/Test, ist von der Produktion getrennt, erlaubt Teilen mit dem gesamten Tenant und unterstützt Backups. Trial ist auf einen Nutzer beschränkt und läuft nach 30 Tagen ab, Dataverse for Teams ist auf Team-Mitglieder beschränkt, die Default-Umgebung kann nicht gesichert werden.

---

### Frage 47
**Frage:** A company uses a set of model-driven apps within a single environment in Microsoft Power Platform.

You need to share a new model-driven app with users.

What should you assign to users to enable them to access the app?
**Antwortmöglichkeiten:**
- Data loss prevention (DLP) policy
- Microsoft 365 security group
- App security role
- Business process flow

**Gewählte Antwort (1. Versuch):** App security role ✅ (richtig)
**Korrekte Lösung:** App security role
**Erklärung:** Model-driven Apps nutzen rollenbasierte Sicherheit; Nutzern muss eine App-Security-Role zugewiesen werden, um Zugriff auf App, Funktionen und Daten zu erhalten.

---

### Frage 48
**Frage:** A coworker requires a personal Microsoft Power Platform environment to test preview features of Power Apps. The coworker wants to use this environment for at least two months.

You need to recommend which type of environment the coworker should create.

Which type of environment should you recommend?
**Antwortmöglichkeiten:**
- Default
- Production
- Developer
- Trial

**Gewählte Antwort (1. Versuch):** Production ❌ (falsch)
**Korrekte Lösung:** Developer
**Erklärung:** Eine Developer-Umgebung ist für den persönlichen Gebrauch des Besitzers gedacht und bleibt bestehen, solange sie aktiv genutzt wird – ideal für längerfristiges Testen von Preview-Features. Trial läuft nach 30 Tagen ab, die Default-Umgebung kann nicht einzeln erstellt werden, Production ist für dauerhaften Betrieb, nicht für Preview-Tests gedacht.

---

### Frage 49
**Frage:** You have a Power Platform production environment that contains a solution.

You create a copy of the production environment and make changes to the solution in the copy.

You need to deploy all the changes from the copy back to the production environment. The solution must minimize administrative effort.

What should you do?
**Antwortmöglichkeiten:**
- Create a new solution in the copy. Export the solution and then import it into the production environment.
- Export all unmanaged customizations from the copy and import them into the production environment.
- Export the solution from the copy and import the solution into the production environment.
- Sync all customizations from the copy to the production environment.

**Gewählte Antwort (1. Versuch):** Export the solution from the copy and import the solution into the production environment. ✅ (richtig)
**Korrekte Lösung:** Export the solution from the copy and import the solution into the production environment.
**Erklärung:** Der Export/Import der (bestehenden) Solution verpackt Änderungen konsistent und minimiert den Verwaltungsaufwand. Eine neue Solution ist unnötig, unmanaged Exports sind für strukturiertes ALM ungeeignet, und eine automatische Sync-Funktion zwischen Umgebungen existiert nicht.

---

## Teilgebiete, an denen ich noch arbeiten muss

Der letzte Screenshot (Testergebnis-Übersicht) zeigt folgendes Gesamtbild:

> "To be better prepared for the exam, aim to achieve a score of 80% or higher in multiple attempts."

**Gesamtergebnis: 52 %** (Ziel: 80 %+)

Die Ergebnisse werden im Test nur als Balkendiagramm ohne exakte Prozentzahl angezeigt. Die folgenden Werte sind aus der Position der Markierung auf der Balkenskala abgeleitet (Kalibrierung anhand des bekannten Referenzpunkts "Score: 52 %") und daher Näherungswerte:

| Teilgebiet (Skill Area) | geschätzter Wert | Einschätzung |
|---|---|---|
| Describe the business value of Microsoft Power Platform | ~90 % | ✅ Stärke – bereits im/nahe dem Zielbereich |
| Demonstrate the capabilities of Power Pages | ~57 % | ⚠️ mittel – Ausbaufähig |
| Demonstrate the capabilities of Power Automate | ~50 % | ⚠️ mittel/schwach |
| Demonstrate the capabilities of Power Apps | ~36 % | ❌ Schwachstelle |
| Manage the Microsoft Power Platform environment | ~33 % | ❌ größte Schwachstelle |

### Konkrete Handlungsempfehlung
1. **Manage the Microsoft Power Platform environment** (schwächster Bereich, ~33 %): Schwerpunktthemen aus diesem Versuch, die falsch beantwortet wurden – Umgebungstypen (Sandbox vs. Trial vs. Developer vs. Default), Security Roles / Least Privilege (Environment Maker vs. System Customizer/Administrator), DLP-Richtlinien zur Connector-Steuerung, Solution-Export/-Import zwischen Umgebungen (Fragen 20, 44, 45, 48).
2. **Demonstrate the capabilities of Power Apps** (~36 %): Unterschied Canvas- vs. Model-driven Apps und passende Datenquellen (Azure SQL, Dataverse), Steuerelemente (Gallery vs. Form vs. Data Table), Farbeigenschaften (Fill vs. Color), Views/Forms-Konfiguration (Fragen 2, 9, 10, 11, 13, 15).
3. **Demonstrate the capabilities of Power Automate** (~50 %): Flow-Typen (Instant/Automated/Scheduled), Desktop Flows und Geräteregistrierung, Business Rules vs. Business Process Flows, Trigger-Auswahl je Szenario (Fragen 23, 27, 30, 39, 43).
4. **Demonstrate the capabilities of Power Pages** (~57 %): Vorlagen-Typen (Solution/Starter/Blank), Site-Migration zwischen Umgebungen über Solutions, Custom Page Templates mit HTML/CSS/Liquid (Fragen 15, 20, 21).
5. **Describe the business value of Microsoft Power Platform** (~90 %) ist bereits solide – hier reicht Auffrischen zur Sicherung.

**Fazit:** Der größte Hebel für die nächste Wiederholung liegt in den Themen **Umgebungsverwaltung (Environments, Security Roles, DLP, ALM)** und **Power Apps-Grundlagen (Canvas vs. Model-driven, Steuerelemente, Formulare)** – hier lagen die meisten falschen Antworten.
