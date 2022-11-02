[ES](./LEERME.md)
[EN](./README.md)

# Application web pair-à-pair: un kata disruptif

## Internet est décentralisé, pourquoi aurions nous besoin de plus de pair-à-pair ?

Dans son design originel et dans son usage le plus fréquent, les technologies
web ont recours à une architecture client serveur. Aussi, le protocole `http`
est fortement teinté de ce paradigme.

Cela n'est pas incompatible avec l'architecture décentralisée du réseau internet
puisqu'il n'y a pas un seul serveur. Il peut y avoir une multitude de serveurs
auquels un client web (browser) peut se connecter. Les serveurs peuvent
d'ailleurs communiquer entre eux, ils peuvent être redondant et il peut
y avoir une multitude de routes permettant d'y accéder.

D'autre part, ce design décentralisé laissait présager que n'importe qui
pourrait participer à ce réseau. Et il est vrai que n'importe qui peut
aujourd'hui publier du contenu.

Mais comment faire si vous ne contrôlez pas un serveur publiquement
accessible sur internet?

![xkcd: the file transfer problematic](https://imgs.xkcd.com/comics/file_transfer.png)

Or, ce design a des conséquences quand à la possibilité de partager
ses données. Et, comme nous le constatons aujourd'hui, le recours
à des intermédiaires pour publier ou transiger nos données a
des conséquences.

## Qu'y a-t-il d'intéressant dans ce kata?

Dans ce kata, nous allons voir de quelles manières il est possibles
d'avoir une connection directe en pair-à-pair entre deux applications
clientes web.

Aussi, nous explorerons ainsi les limites de cette approche, verrons quelles
conséquences imposent le design actuel d'internet et comment il est possible
de contourner ces limites.

## Application type

Voici les requis généraux d'une application web cliente pair-à-pair:

  - Deux clients web ou plus souhaitent communiquer entre eux sans avoir besoin
    de passer par un système tier.
  - Les clients web ne dispose pas nécessairement d'une connection à internet,
    ils peuvent être connectés:
    - à un même réseau,
    - à deux réseaux qui possèdent une connection entre eux, ou
    - à aucun réseau.
  - Les deux clients web parviennent à établir une connection.
  - Il serait préférable que les deux clients valident leur identité.
  - À la suite de quoi, les 2 clients échangent de l'information qui a de
    la valeur pour les utilisateurs.







