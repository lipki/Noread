Noread
======

Un simple favoris pour masquer les vidéos vues sur NOCO


Glisser déposer ce lien 
[NOCO-noread](javascript:(function(){if($('.tr').length==0){$('#menu-right').append('<ul><li><img%20id="tr"%20class="tr"%20src="http://noco.tv/cdata/images/mark-read.png"%20style="vertical-align:%20sub;%20padding:%204px%2010px;"></li></ul>');b%20=%20$('#tr');b.v=true;b.click(function(){b.v=!b.v;if(b.v){b.parents('ul').css('background','none');$('.mark_read').show('slow')}else{b.parents('ul').css('background','#9EC70F');$('.mark_read').hide('slow')}})}})())

--> ]NOCO-noread[/url] <-- dans votre barre de favori.
Une fois sur Noco, un clic sur ce favoris, fera apparaitre un bouton à côté du moteur de recherche (avec un œil dedans), pour afficher/masquer les vidéos vues.

Testé pendant deux minutes sur un seul navigateur. Garanti sans bug connu :D

Pour les curieux voici le code.
[code]
javascript:(function(){
    if($('.tr').length==0){
        $('#menu-right').append('<ul><li><img id="tr" class="tr" src="http://noco.tv/cdata/images/mark-read.png" style="vertical-align: sub; padding: 4px 10px;"></li></ul>');
        b = $('#tr');
        b.v=true;
        b.click(function(){
            b.v=!b.v;
            if(b.v){
                b.parents('ul').css('background','none');
                $('.mark_read').show('slow')
            }else{
                b.parents('ul').css('background','#9EC70F');
                $('.mark_read').hide('slow')
            }
        })
    }
})()
[/code]
