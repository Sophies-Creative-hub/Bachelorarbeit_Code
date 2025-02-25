# Bachelorarbeit_Code

STDP auf die technische Umsetzung stärker beziehen.
Variablen auf Seite 9 direkt ausführlicher erklären.
Aufstellung was heißt jede Variable, englischen Begriffe nutzen zu Beginn!

Gesamtbild auf Neuronen beziehen, erst dann Formeln
Nochmal darstellen, wann feuert ein Neuron? präsynaptisches feuern beeinflusst durch presynaptisches


synaptische Gewicht W vorher auch erwähnen => Gewichtsmatrix (?) 

Berechnung P/Q unabhängig voneinander

,,τLTD regelt, wie schnell dieser
Einfluss abklingt, und ALTD bestimmt, wie stark die Verbindung bei Depression – also wenn der
postsynaptische Spike vor dem prä-synaptischen kommt – abgeschwächt wird." --> gilt für beide Formeln

wann wird welche Formel zum Einsatz?

wie bestimmt man, welches Neuron zuerst feuert?

ggf. auch ein Bild

! auf a ändern ,, Die Verstärkungsfaktoren ALTP
und ALTD bestimmen dabei, wie stark eine Veränderung der Verbindung ausfällt."

Beispiel 1+2 passieren immer, und Beispiel 3+4 greifen nur in bestimmmten Fällen, nochmal in der Quelle nachlesen => Pseudocode verwenden

Beispielwerte Seite 4 nutzen!

Beispiele 1 + 3 zusammenfassen, Beispiele 2 + 4 zusammenfassen zu Depression/Potention -> Werte anpassen --> das postsynaptische muss SPÄTER feuern

Beispiel 1 --> Teil a und Teil b

t'pre --> vorher

dann müsste der Exponent doch negativ sein

δWp = aLTP·P·exp
tpre−tpost
τLTP

Delta W? --> immer positiv

"Eqs. (1)-(4) describe the STDP rule [23] used in this
work. In this rule, the weight changes are proportional to
spike trace [24]. tpre and tpost denote the time a pre- and
post-synaptic, respectively, spikes arrive; tpre′ and tpost′
represent the arrival time of previous pre- and post-synaptic
spikes respectively. ALTP and ALTDare the amplitudes of
trace updating for potentiation and depression respectively;
and aLTP and aLTD are the potentiation and depression
) + ALTP (1)
) + ALTD (2)
learning rate respectively. Each pre-synaptic spike arrival will
update the pre-synaptic trace P according to Eq. (1), post-
synaptic spike changes the post-synaptic trace Qaccording to
Eq. (2). If a pre-synaptic spike happens after a post-synaptic
spike, weight will decrease by δW q , which is given by (3). If
a post-synaptic spike occurs after a pre-synaptic spike, weight
will increase by δW p given by (4).
P= P ×exp( tpre′−tpre
τLT P
Q= Q×exp( tpost′−tpost
τLT D
δW q= aLTD×Q×exp( tpost−tpre
),tpost <tpre (3)
τLT D
δW p= aLTP ×P ×exp( tpre−tpost
),tpre <tpost (4)" Zu Beginn

ZU BEGINN


,,STDP sorgt also dafür, dass sich die Verbindungen zwischen Neuronen dynamisch anpassen –
immer basierend auf dem Timing der Spikes. Wenn die Neuronen gut synchron feuern, verstärken
sie ihre Verbindung. Wenn sie asynchron feuern, schwächen sie diese Verbindung. So ermöglicht
STDP, dass das Gehirn auf der Grundlage von Erfahrung und zeitlichem Zusammenspiel lernt
und sich immer wieder anpasst"

und dann Rückbezug Hebbsches Lernen mit Zitata

--> im Bewertungskapitel auf fehlende Möglichkeit der Implementation dazu eingehen


2.2

vor einigen Jahren --> Ersetzung Jahreszahl

Encoder --> was bedeutet die y-Achse? Durchnummerierung der Neuronen oder Stromwert?

--> warum validation 

training accuracy vs Test accuracy

training vs validation

bei Gegenüberstellungen --> gleiche Skalen

15 Stunden -> FMnist nochmal nachschauen

N-MNIST -> Ergebnisübersicht