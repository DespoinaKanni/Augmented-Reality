# Lesson: Interaction Design

### First and Last Name: xxx
### University Registration Number: dpsdxxxxx
### GitHub Personal Profile: xxx
### Augmented Reality Personal Repository: 

# Introduction

# Summary


# 1st Deliverable
Η εργασία πραγματοποιήθηκε στους υπολογιστές της σχολής.
Αρχικά συνδέθηκα στο GitHub με τους προσωπικούς μου κωδικούς. Από το προφίλ μου μπήκα στο Augmented-Reality όπου εκεί πάτησα στο Code (πράσινο χρώμα) και επέλεξα να ανοίξει με το GitHub Desktop (Open with GitHub Desktop). Χρειάστηκε να εγκαταστήσω το GitHub Desktop στον υπολογιστή και αφού το έκανα συνδέθηκα με τους προσωπικούς μου κωδικούς. Στην συνέχεια ακολούθησα την διαδρομή zdrive\Documents\GitHub\Augmented Reality\ marker_based και εκεί βρήκα το αρχείο index όπου το άνοιξα με Visual Studio και εμφανίστηκε ο κώδικας. Στην συνέχεια από την αναζήτηση (search bar windows) εντόπισα το Command Prompt και ακολούθησα τις παρακάτω ενέργειες:
Z:\>cd “My Documents” (enter) 
Z:\My Documents>cd GitHub (enter)
Z:\My Documents\GitHub>cd Augmented-Reality (enter)
Z:\My Documents\GitHub\Augmented-Reality>python -m http.server (enter)

Το python -m http.server το βρήκα μέσα από: merkourisa/Augmented-Reality στα Discussions στο Preview του κώδικα και το αντέγραψα και το έκανα επικόλληση στο Command Prompt
Τέλος, πάλι μέσα από το Preview του κώδικα πάτησα το  http://localhost:8000/ όπου μου άνοιξε την κάμερα του υπολογιστή.

Έπειτα, επέστρεψα ξανά στο αρχείο με τον κώδικα στο Visual Studio για να τον συμπληρώσω με τις νέες εντολές.
Για το κουτί χρησιμοποίησα την ήδη υπάρχουσα εντολή που μας δινόταν και άλλαξα τα νούμερα στο  width, depth, height.
Για τον κύλινδρο και την σφαίρα έψαξα στο διαδίκτυο https://medium.com/analytics-vidhya/a-frame-changing-environment-tutorial-a71bc69202d4
για να βρω τον κώδικα που αντιστοιχεί για το καθένα και το προσάρμοσα στο αρχείο κάτω από την εντολή του box

<a-entity id="box" geometry="primitive: box; width: 0.4; depth: 0.3; height: 0.4" position="0 0 0"
                      material="color: #4CC3D9"></a-entity>

<a-entity id="cylinder" geometry="primitive: cylinder;  height: 0.3; radius: 0.2" position="-0.5 0 0"
                      material="color: #cdb5f7"></a-entity>

<a-entity id="sphere" geometry="primitive: sphere; radius: 0.1" position="0.5 0 0"
                      material="color:#10e670"></a-entity>

Τα χρώματα τα άλλαξα από το internet για το #cdb5f7 https://www.google.gr/search?q=%23cdb5f7&sxsrf=APq-WBuCsZkOJofs0UVSw8lEl-aS4X9sOg%3A1647974436656&source=hp&ei=JBg6Yq-tJcKQxc8P-oauYA&iflsig=AHkkrS4AAAAAYjomNB-5rZW3gtRtOHQfyqIx_FHVlLai&ved=0ahUKEwivz5KXr9r2AhVCSPEDHXqDCwwQ4dUDCAc&uact=5&oq=%23cdb5f7&gs_lcp=Cgdnd3Mtd2l6EAM6BwgjEOoCECdQ1eyBBFjV7IEEYPb3gQRoAXAAeACAAZ0CiAGdApIBAzItMZgBAKABAqABAbABCg&sclient=gws-wiz

και για το #10e670
https://www.google.gr/search?q=%2310e670&sxsrf=APq-WBtejlm9TU_fqOYZft7HuOrm-dBfVA%3A1647982858358&ei=Cjk6Yu-0FZabkgX12qz4Dw&ved=0ahUKEwjv4fjGztr2AhWWjaQKHXUtC_8Q4dUDCA4&uact=5&oq=%2310e670&gs_lcp=Cgdnd3Mtd2l6EAM6BwgjEOoCECdKBAhBGABKBAhGGABQAFjEFmDyKmgBcAB4AIABowGIAaMBkgEDMC4xmAEAoAEBoAECsAEKwAEB&sclient=gws-wiz



Τέλος, πρόσθεσα τα χιόνια και τις φωνητικές εντολές από τα λινκ https://www.npmjs.com/package/aframe-particle-system-component
https://www.npmjs.com/package/aframe-speech-command-component
που το βρήκα από το  DespoinaKanni/Augmented-Reality στο Deliverable 1


<a-entity id="annyang" annyang-speech-recognition></a-entity>
<a-entity id="switch" speech-command__start="command: start; type: attribute; attribute: visible; targetElement: #snow; value: true;"
             speech-command__stop="command: stop; type: attribute; attribute: visible; targetElement: #snow;  value: false;">
</a-entity>
<a-entity id="snow" position="0 6 -15" particle-system="color: #ffffff"></a-entity>

Αφού τελείωσα τον κώδικα πάτησα save στο Visual Studio για να αποθηκευτούν οι αλλαγές και πήγα στην κάμερα να δω εάν λειτουργεί. Έκανα ένα refresh και μου εδειξε στην οθόνη τον εαυτό μου και να πέφτουν τα χιόνια ,έβαλα μπροστά από την κάμερα το χαρτί με το hiro και εμφανίστηκαν στην οθόνη το κουτί, ο κύλινδρος και η σφαίρα. Τέλος φώναξα την λέξη STOP για να σταματήσει να πέφτει το χιόνι και την λέξη START για να ξεκινήσει ξανά. Όμως, αργούσε λίγο και καμια φορά δεν το αντιλαμβανόταν με την πρώτη  ή έπρεπε να φωνάξω δυνατά. Αφού τελείωσα την εργασία μπήκα στο GitHub Desktop για να στείλω την εργασία μου στο GitHub πάτησα commit main και μετά push origin.



# 2nd Deliverable


# 3rd Deliverable 


# Conclusions


# Sources
