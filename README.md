Οπτικοποίηση Δεδομένων Χορηγιών (UK)</br>
Τριανταφυλλίδης Βασίλης Π2013135</br>
Μάθημα "Τεχνολογία Λογισμικού"</br>

Θέμα Εργασίας: Οπτικοποίηση Δεδομένων Χορηγιών (UK) - Data Visualization</br>

Εξάμηνο Φοίτησης    :    Επί Πτυχίω</br>
E-mail              :    p13tria@ionio.gr

Aποθετήριο του κώδικα (p13tria)       :       https://github.com/p13tria/D3js-uk-political-donations</br>
Link εκτελέσιμου                      :       https://p13tria.github.io/D3js-uk-political-donations</br>
Link 1ου Παραδοτέου                   :       https://github.com/p13tria/D3js-uk-political-donations/tree/gh-pages</br>

Παραδοτέο 1

Για την αλλαγή των χρωμάτων στις μπάλες με τα δεδομένα προχώρησα σε τροποποίηση του κώδικα του chart.js

![Chart1](https://github.com/p13tria/sw/blob/2013135/projects/2013135/Chart1.png)
https://github.com/p13tria/D3js-uk-political-donations/blob/gh-pages/chart.js

Για την αλλαγή στον ήχο κάθε φορά που γίνεται κλικ προχώρησα σε τροποίηση του κώδικα του index.html (αφού πρώτα το μεταονόμασα όπως ζητήθηκε στο παραδοτέο απο full-viz.html σε index.html)
https://github.com/p13tria/D3js-uk-political-donations/blob/gh-pages/index.html

```javascript
<script>
    var button_sound = new Audio();
    button_sound.src = "ButtonSound.mp3";
    </script>
```
και 

```javascript
<ul>
            <li><a href="#" onmousedown="button_sound.play()" role="button" class="pure-button switch" id="all-donations">All money</a>
            </li>
            <li><a href="#" onmousedown="button_sound.play()" role="button" class="pure-button switch" id="group-by-money-source">The public's purse</a>
            </li>
            <li><a href="#" onmousedown="button_sound.play()" role="button" class="pure-button switch" id="group-by-party">Split by party</a>
            </li>
            <li><a href="#" onmousedown="button_sound.play()" role="button" class="pure-button switch" id="group-by-donor-type">Split by type of donor</a>
</ul>  
```        
Για άνοιγμα νέου παράθυρου με κλικ σε κάποια μπάλα, με το αποτέλεσμα google search για τον δωρητή της κλικαρισμένης μπάλας, προχώρησα σε τροποποίηση στο chart.js. 
https://github.com/p13tria/D3js-uk-political-donations/blob/gh-pages/chart.js
```javascript
" .on("click", function(d) { window.open("http://www.google.com/search?q=" + d.donor);});
```

Ζητούμενα στα οποία απαιτούνται αλλαγές (pull request) στο κοινό αποθετήριο του κώδικα
Δημιουργήθηκε αρχείο 2013135.csv στο φάκελο participants με κάποια απαραίητα στοιχεία που ζητήθηκαν.
Τοποθετήθηκαν 5 εικόνες για τους εξής δωρητές:  Cellcrypt
                                                Folkes Holdings
                                                Gerald Andrews
                                                Southwark Labour Group
                                                Tangent Communications
