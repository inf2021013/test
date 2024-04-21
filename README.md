# Info Tab

## General App Information

Η συγκεκριμένη εφαρμογή χρησιμοποιείται για την `οπτικοποίηση δεδομένων` και `σύγκριση αλγορίθμων μηχανική μάθησης` όπου για να επιτευχθεί αυτή η λειτουργία γίνεται χρήση του εργαλείου Streamlit. Πιο συγκεκριμένα, η εφαρμογή υποστηρίζει διάφορες λειτουργίες όπως φόρτωση `tabular` δεδομένων (.csv), προδιαγραφές πινάκων `(dataframes)`, `2D οπτικοποιήσεις` βασισμένες σε διαφορετικούς αλγορίθμους, `μηχανική μάθηση` όπου δίνονται δύο επιλογές ειδών αλγορίθμων για τον χρήστη (`κατηγοριοποίησης` ή `ομαδοποίησης`) όπου μπορεί να πραγματοποιηθεί και `σύγκριση` των προαναφερόμενων αλγορίθμων με σκοπό την εύρεση του `πιο αποδοτικού` και τέλος μια παρουσίαση του τρόπου λειτουργίας της εφαρμογής (Η συγκεκριμέση σελίδα).

## How to Use it?

Η χρήση της εφαρμογής είναι απλοϊκή και εύκολα κατανοητή για όλους. Αρχικά ο χρήστης θα χρειαστεί να ανεβάσει τα δεδομένα που θέλει σε μορφή `CSV, Excel`. Έπειτα από αυτό ο χρήστης μπορεί να αποφασίσει ποια λειτουργία της εφαρμογής θέλει να εκμεταλευτεί. Στα αριστερά του ανοιχτού παραθύρου βρίσκονται οι ακόλουθες επιλογές: `DataFrame_tab, Visualization_tab, Machine_Learning_tab, Info_tab` με κάθε μια από αυτές να εκτελεί μια διαφορετική λειτουργία με λεπτομερής περιγραφή παρακάτω:

### Data Frame tab:

Εάν ο χρήστης ενδιαφέρεται για την `εμφάνιση του Dataset` του σε μορφή πινάκων τότε επιλέγοντας την DataFrame_tab μπορεί να το επισκοπήσει. Αρχικά του δίνεται η επιπλέον επιλογή για τον τρόπο παρουσίασης του Data set με ή χωρίς labels. 

#### labels επιλογή
Αν επιλέξει την επιλογή labels τότε θα εμφανίσει μερικές πληροφορίες για το Dataset (όπως τον αριθμό γραμμών - στηλών, τα unique labels του Dataset και τα πόσα είναι).

![dataframe_info_labels](https://github.com/inf2021013/test/assets/166173503/fafaff30-d07b-4302-a49e-7caf99f5061f)

Έπειτα του δίνεται η δυνατότητα να ανοίξει και να κλείσει το Data set αφότου ολοκληρώσει την επισκόπηση του.

![image](https://github.com/inf2021013/test/assets/166173503/e7d30dd1-a6eb-4a8e-8cf5-66eb96986ea1)

Τέλος, διαχωρίζει το Dataset του δύο κομμάτια, σε `Samples X Features` και `Labels` παίρνοντας την τελευταία στήλη του Dataset
![dataframe_labels](https://github.com/inf2021013/test/assets/166173503/b6abd089-b0bd-43bf-b307-4f77eb2f5705)


#### no labels επιλογή
Αν επιλέξει την επιλογή no labels τότε θα εμφανίσει τον αριθμό γραμμών - στηλών του Dataset.

![dataframe_info_no_labels](https://github.com/inf2021013/test/assets/166173503/c36d1950-2bc9-492b-ba0e-f5e9722f5a64)

Έπειτα του δίνεται η δυνατότητα να ανοίξει και να κλείσει το Data set αφότου ολοκληρώσει την επισκόπηση του.

![image](https://github.com/inf2021013/test/assets/166173503/e7d30dd1-a6eb-4a8e-8cf5-66eb96986ea1)

Τέλος, εμφανίζει ολόκληρο το Dataset, σε `Samples X Features`.

![dataframe_info_no_labels](https://github.com/inf2021013/test/assets/166173503/5ef0439a-2500-41bc-b8ed-2e1e99f90a5d)

### Visualization tab:

Εάν ο χρήστης επιθυμεί να εκτελέσει 2D οπτικοποιήση βασισμένη σε δύο αλγορίθμους μείωσης διάστασης (PCA,t-SNE) μπορεί να επιλέξει την Visualization_tab. Εδώ με την χρήση των δεδομένων που παρείχε στο αρχικό βήμα ο χρήστης δημιουργούνται και εμφανίζονται οι οπτικοποιήσεις τους ανάλογα με τον αλγόριθμο που έχει επιλέξει.

- Οι δύο αλγόριθμοι που προσφέρονται είναι οι PCA και t-SNE.
- Επιπρόσθετα παρουσιάζονται 3 διαγράμματα exploratory data analysis (EDA), αναλυτικότερα, ένα ιστόγραμμα (Histogram), ένα διάγραμμα πυκνότητας (Density) και ένα διάγραμμα Boxplot βασιμσένα στα παρεχόμενα δεδομένα του χρήστη.

### Machine Learning tab:

Εάν ο χρήστης θέλει να υλοποιήσει και να συγκρίνει αλγορίθμους Μηχανικής Μάθησης μπορεί να επιλέξει το Machine_Learning_tab. Εδώ του δίνεται η δυνατότητα να διαλέξει ανάμεσα σε αλγορίθμους κατηγοριοποίησης (Support Vector Machines, K-Nearest Neighbors) και αλγορίθμους ομαδοποίησης (Agglomerative Clustering, Affinity Propagation). Αφότου επιλέξει τους επιθυμητούς αλγορίθμους χρειάζεται να παρέχει τιμή για την μεταβλητή κάθε αλογρίθμου

#### **Αλγορίθμοι Κατηγοριοποίησης:**

**Xρειάζεται να παρέχει:**

- **α)** την regularization παράμετρο για τον Support Vector Machines,
- **β)** των k αριθμό γειτόνων για την K-Nearest Neighbors

#### **Αλγορίθμοι Ομαδοποίησης:**

**Xρειάζεται να παρέχει:**

- **α)** των αριθμό των clusters για τον Agglomerative Clustering,
- **β)** το bandwidth της παραμέτρου για τον Affinity Propagation Clustering.

Επιπλέον μπορεί να συγκρίνει την αποδοτικότητα των αλγορίθμων και να βρει τον πιο αποδοτικό για κάθε περίπτωση πατώντας το **"Start Analysis"**. Έπειτα από ενα μικρό χρονικό διάστημα θα εμφανιστούν οι αποδόσεις των δύο επιλεγμένων αλγορίθμων καθώς και ποιος από τους δύο είχε την καλύτερη απόδοση και το ποσοστό της ακρίβειας του.

### Info tab:

Τέλος εάν ο χρήστης χρειάζεται βοήθεια για τον τρόπο λειτουργίας της εφαρμογής ή θέλει να δει γενικές πληροφορίες για αυτήν μπορεί να επιλέξει την Info_tab. Εδώ προσφέρονται γενικές πληροφορίες της εφαρμογής, ο τρόπος λειτουργίας της και η ομάδα ανάπτυξής της καθώς και ποια tasks ανέλαβε και ολοκλήρωσε κάθε μέλος της.

## Team Members

Η ομάδα ανάπτυξης της εφαρμογής αποτελείται από τον Νικόλα Αναγνωστόπουλο, τον Αχιλλέα Ζερβό και τον Παναγιώτη Μουρελάτο, φοιτητές του Ιονίου Πανεπιστημίου στο 3ο έτος της φοιτησής τους.

## Tasks Completed by each member

- ### Data Frame
  Την ανάπτυξη του Data Frame ανέλαβε και ολοκλήρωσε ο Νικόλας Αναγνωστόπουλος με ΑΜ: inf2021013
- ### Visualization
  Την ανάπτυξη του Visualization ανέλαβε και ολοκλήρωσε ο Αχιλλέας Ζερβός με ΑΜ: inf2021055
- ### Machine Learning
  Την ανάπτυξη του Machine Learning ανέλαβε και ολοκλήρωσε ο Νικόλας Αναγνωστόπουλος με ΑΜ: inf2021013
- ### Info
  Την ανάπτυξη του Info ανέλαβε και ολοκλήρωσε ο Παναγιώτης Μουρελάτος με ΑΜ: inf2021147
