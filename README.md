# Staccioli Doc

**nota bene** There is another, probably more updated version, on: [GitLab](https://gitlab.mpcdf.mpg.de/kewerner/staccioli-doc) .

Documentation for the Mauro Staccioli project. Mostly related to the Field Database.

## Database App

The Android/iOS and Win/Mac/Linux app is available here: [MementoDB](https://mementodatabase.com/download.html).

The interface is very efficient and user friendly. Here's a screenshot:

![Java](https://github.com/biblhertz/StaccioliDoc/blob/main/screenshot_FieldDB_Android.png)

The desktop version instead is JAVA based. There are not many differences.

## Database Connection

You have to create an account and then ask the database owner (werner@biblhertz.it) for an invitation. There can be multiple users for data editing and input.

## Database Status

The database contains only the data necessary for the scanning process:

1. box / folder / item numbering
2. item categorizing: important for division of labor between fototeca and library
3. useful things like the possibility to add a snapshot, and notes

## Database Live View

There is a public [Live View](https://dlib.biblhertz.it/staccioli) into the dataset available. Changes are reflected in real-time.

## Database Structure

| Field name | Field type   | Required | Used for                                      |
| ---------- | ------------ | -------- | --------------------------------------------- |
| box        | Text          | true     | Retrivability                                   |
| folder     | Text          | true     | Retrivability                                   |
| number     | Text          | true     | Retrivability                                   |
| type*      | Single-choice | true     | Attribution Fototeca/Library & generic tipology | 
| project**  | Single-choice | true     | Project and Year                                |
| photos     | Image         | false    | General overview (optional)                     |
| title      | Text          | false    | Optional title (mostly for printed material)    |
| note       | Text          | false    | Comment                                         |


* Possible values for `type` are:  

| Type     | AAT      | Department |
| -------- | -------- | ---------- |
| booklet | [300311670](http://vocab.getty.edu/page/aat/300311670) | Library |
| admission ticket | [300133073](http://vocab.getty.edu/page/aat/) | Library |
| contact sheet | [300127183](http://vocab.getty.edu/page/aat/300127183) | Fototeca |
| correspondence | [300026877](http://vocab.getty.edu/page/aat/300026877) | Library |
| document | [300026030](http://vocab.getty.edu/page/aat/300026030) | Library |
| draft | [300026932](http://vocab.getty.edu/page/aat/300026932) | Fototeca |
| drawing | [300033973](http://vocab.getty.edu/page/aat/300033973) | Fototeca |
| etching | [300053241](http://vocab.getty.edu/page/aat/300053241) | Fototeca |
| exhibition catalog | [300026096](http://vocab.getty.edu/page/aat/300026096) | Library |
| exhibition invitation | [300417367](http://vocab.getty.edu/page/aat/300417367) | Library |
| floor plan | [300034158](http://vocab.getty.edu/page/aat/300034158) | Fototeca |
| flyer | [300224742](http://vocab.getty.edu/page/aat/300224742) | Library |
| form | [300049060](http://vocab.getty.edu/page/aat/300049060) | Library |
| invitation | [300027083](http://vocab.getty.edu/page/aat/300027083) | Library |
| journal | [300215390](http://vocab.getty.edu/page/aat/300215390) | Library |
| leaflet | [300211825](http://vocab.getty.edu/page/aat/300211825) | Library |
| lithograph | [300041379](http://vocab.getty.edu/page/aat/300041379) | Fototeca |
| location map | [300028373](http://vocab.getty.edu/page/aat/300028373) | Fototeca |
| logo | [300028715](http://vocab.getty.edu/page/aat/300028715) | Fototeca |
| manifesto | [300026393](http://vocab.getty.edu/page/aat/300026393) | Library |
| negative | [300127173](http://vocab.getty.edu/page/aat/300127173) | Fototeca |
| newspaper | [300026656](http://vocab.getty.edu/page/aat/300026656) | Library |
| newspaper clipping | [300429554](http://vocab.getty.edu/page/aat/300429554) | Library |
| notes | [300027200](http://vocab.getty.edu/page/aat/300027200) | Fototeca |
| photographic print | [300127104](http://vocab.getty.edu/page/aat/300127104) | Fototeca |
| photomontage | [300419270](http://vocab.getty.edu/page/aat/300419270) | Fototeca |
| planimetric map | [300028098](http://vocab.getty.edu/page/aat/300028098) | Fototeca |
| postcard | [300026816](http://vocab.getty.edu/page/aat/300026816) | Fototeca |
| press release | [300026437](http://vocab.getty.edu/page/aat/300026437) | Library |
| project | [300048788](http://vocab.getty.edu/page/aat/300048788) | Fototeca |
| prospect view | [300264665](http://vocab.getty.edu/page/aat/300264665) | Fototeca |
| regulation | [300027843](http://vocab.getty.edu/page/aat/300027843) | Library |
| scale model | [300266034](http://vocab.getty.edu/page/aat/300266034) | Fototeca |
| section drawing | [300034223](http://vocab.getty.edu/page/aat/300034223) | Fototeca |
| sketch | [300015617](http://vocab.getty.edu/page/aat/300015617) | Fototeca |
| slide | [300128371](http://vocab.getty.edu/page/aat/300128371) | Fototeca |
| typescript | [300028577](http://vocab.getty.edu/page/aat/300028577) | Library |

Please note that the division of labor between Fototeca and Library is not yet finally discussed (eg. regarding handwritten notes {300027200}).  

** Possible values for `project` are:

| Evento |
| -----------------------|
| Aptico Il senso della scultura 1976 |
| AR.GE.ALP Milano 1977  |
| Arte e critica Roma 1981 |
| Arte e didattica Forlì 1977  |
| Arte e lavoro Suzzara 1974 |
| Aurea Arte Firenze 1979  |
| Biennale di Milano Milano 1974  |
| Biennale di Venezia 1978 |
| Biennale di Venezia Venezia 1976  |
| Bruxelles 1977 |
| Casa Gandola Como 1976  |
| Condizione Cile Galleria di Porta Ticinese Milano 1974 |
| Cooperativa esperienze culturali Bari 1978 |
| Expo Arte Studio Carrieri Bari 1980 |
| Festival dell’unità Mantova 1978  |
| Fondazione Michetti Francavilla al mare 1977  |
| Galleria Bocchi Milano 1975  |
| Galleria Comunale d’Arte Moderna Cagliari 1975  |
| Galleria Il gelso Lodi 1975-1976  |
| Galleria Inquadrature 33 Firenze 1971 |
| Galleria San Fedele Milano 1971 |
| Galleria Spriano Omegna 1981 |
| Galleria Stefanoni Lecco 1974 |
| Galleria Studio Varsavia 1980 |
| Galleria Toninelli Milano 1972  |
| Gibellina 1979  |
| Gli ultimi quindici anni di arte in Italia Museo Civico Torino 1977 |
| Gubbio ’76 Biennale della ceramica metallo e altri materiali Gubbio 1976  |
| Il luogo della forma Museo di Castelvecchio Verona 1981 |
| Il luogo di lavoro dell’arte Studio Alik Milano 1981 |
| Incontri di Martinafranca Martinafranca 1979  |
| Interventi nello spazio urbano Torino 1974 |
| Intox Grenoble 1971 |
| La critica dell’arte Galleria d’Arte Moderna Palazzo Bosardi Ancona 1981 |
| La section d’or Loggetta lombardesca Ravenna 1979 |
| Lettura di un ambiente Vigevano 1977 |
| LIS ’79 Lisbona 1979 |
| Lombardia: vent’anni dopo Castello visconteo Pavia 1981 |
| Mauro Staccioli. Il segno come scultura Galleria Civica d’Arte Moderna Macerata 1981 |
| Mercato del sale Milano 1981 |
| Montreal 1977  |
| Monumento alla resistenza Vigevano 1980 |
| Monumento Franceschi Milano 1975  |
| Orlando al dosso Mantova 1979  |
| Piazza Cermenate Lecco 1979/1980  |
| Piazzale Sant’Agostino Bergamo 1981 |
| Piazzetta Einaudi Milano 1974/1975 |
| Operazione Arcevia Arcevia 1975  |
| Poggio Gagliardo 1979  |
| Premio Comiso Comiso 1977 |
| Premio Pagani Legnano 1972 |
| Salon de la jeune sculpture Parigi 1973 |
| Scultoincontro Verbania 1974  |
| Scultura ’71 Collezione Collegio Cairoli Pavia 1972 |
| Scultura: la città come spazio operativo Pesaro 1976 |
| Sculture contemporanee nello spazio urbano Parma 1973 |
| Sculture in città Volterra 1972 |
| Scuola Caprin Trieste 1980  |
| Sette scultori per Matera Studio D’Ars Milano 1978 |
| Sistemazione della lapide al partigiano Agostino Lenti Valenza Po 1975  |
| Studio Carrieri Martinafranca 1980 |
| Subzara il fiume la gente la festa Suzzara 1980  |
| Studio Marconi Milano 1975 |
| Studio Santandrea Milano 1973 |
| Studio Santandrea Milano 1975 |
| Studio Santandrea Milano 1981 |
| Suzzara 1977  |
| Tomba famiglia Mazzani Cimitero Greco Milano 1980/1981 |
| Una cartolina per Como Como 1978  |
| VII Biennale del metallo Gubbio 1973 |
| Villa Manzoni Lecco 1974  |
| Villa Manzoni Lecco 1981-1982 |
| Volterra ’73 Volterra 1973 |
