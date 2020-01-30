##Esercizio Relazioni

Abbiamo qua di fronte un esempio di crud su post che mette insieme diverse relazioni.

Avremo la tabella posts che sarà collegata ad una e una sola categoria (le categorie invece saranno collegate a diversi post), e ad una ed una sola riga delle post information. Immaginiamo che questa terza tabella (post information) siano delle informazioni aggiuntive che vogliamo dare ai nostri post ma che per motivi di ordine e organizzazione preferiamo inserire in un'altra tabella.

Questo è uno dei codici base che potremmo utilizzare per ripassare questa importante parte di laravel.

Il nostro esercizio consisterà nel:

-   Creare una nuova tabella: Tags
-   Avrà una relazione con posts di tipo many to many.
-   La tabella dovrà avere due campi: title e slug
-   Una volta creata la migration e quindi la tabella aggiungere le funzioni che ci permetteranno di leggere le relazioni
-   Modificare la crud aggiungendo anche i tag

**Bonus**

-   Aggiungere anche i metodi: create, store e show
-   Aggiungere il seeder dei tag
-   Aggiungere la validazione lato client e lato back

##Relations
Category 1 <> N Posts
Posts N <> N Tags
Post 1 <> 1 PostInformation
User 1 <> N Posts

##relazione unique tag_id post_id
usare
php artisan migrate:fresh --seed
perchè refresh da errore

##Possibilità di rimuovere singolo tag da un post(conservando il post stesso)

##Add user_id on post creation

##Authenticantion
composer require laravel/ui --dev

php artisan ui vue --auth

npm install && npm run dev

##show create post only if logged, save user_id on related post

##show edit/delete button only for logged related user

#user image
- ins field 'image' in User table, fillable in model