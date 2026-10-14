# CONTENT.md: all text for aspring.ca (EN default, FR)

Ground truth for the design. Every string that appears on a page is here, in English (default) and French. **The design uses only this text.** Do not invent or reword copy in the design; change it here first.

## Tags

| Tag | Meaning |
|---|---|
| `REAL` | From an approved source: ClinicSense (Victoria's own service text and prices), the approved Welcome email, or confirmed contact details. Safe to use. |
| `DRAFT` | Client's own mockup copy (`client-brief/`). Good voice, but not yet approved by Victoria. Usable in the design. Facts inside must be checked. |
| `FACT` | Contains a number or claim that must match `FACTS.md`. Marked with ⚠ where it currently conflicts. |
| `PLACEHOLDER` | Design-only dummy content (invented names, products, dates). **Never publish.** Exists so the layout can be reviewed. |
| `NEW` | Written now for the structure (not from the client). Needs Victoria's review. |
| `FR-NEW` | French written now, with no client original. Needs a native review. |

Rules applied: the name **Aspring Health Center** (header wordmark: **Aspring Health**); the therapist is **Victoria** (the mockup spells "Viktoria", corrected everywhere); first person for Victoria; no medical or cure claims in new copy.

## Decisions applied

- **Name:** **Aspring Health Center** is used everywhere (footer, copyright, page titles, schema), matching the Google Business Profile. Only the header wordmark says **Aspring Health**.
- **Neck therapy:** kept, because it is a ClinicSense service. The practitioner name in the ClinicSense text ("Andrey Aspring") is not used anywhere on the site. Victoria should correct the ClinicSense description, and confirm who performs the service.
- **Health claims softened** in all website service descriptions (no "scientifically proven", percentages, "break down deposits", "lasting results", "eliminate the true causes").
- **Mockup services not on ClinicSense are dropped** (Therapeutic Swedish, Prenatal, Ayurvedic Abhyanga as a bookable type, the mockup price table).

## Still open

- **Years of experience** are inconsistent (mockup "15+", approved email "nine years", old site 9+/7/5+). The home hero, stats, credentials chip and the Sleep talk use the mockup's "fifteen years". One number is needed in `FACTS.md`.
- **Testimonials in the mockup are invented** (Marie-Claude L., Daniel R., Sophie B.). Use real Google reviews with permission.
- **Credentials table is a guess** (issuing bodies, years). Needs Victoria's real credentials.
- **Hours:** mockup says "Tue – Sat" and "Evenings and Saturdays". Real hours per the approved email: Mon–Sun 9 am–9 pm. Confirm in `FACTS.md`.
- **Unverified claims:** insurance receipts and acceptance, "direct billing not required", "packages of five", "24-hour cancellation", "Taxes included".
- **Retreats, events, library and shop** are the client's draft items: `DRAFT`/`PLACEHOLDER` until she confirms real dates, prices and products.
- **Monsalada**: "first certified Monsalada practitioner in Canada" appears in the approved email but is not used in the softened service text until confirmed.

## 0. Global (header, footer, buttons, forms)

### Header

**Wordmark**  `REAL`
- EN: Aspring Health
- FR: Aspring Health

**Tagline under wordmark**  `DRAFT`
- EN: Holistic Care · Montréal
- FR: Soins holistiques · Montréal

**Nav: massage**  `DRAFT`
- EN: Massage Therapy
- FR: Massothérapie

**Nav: holistic**  `DRAFT`
- EN: Naturopathy & Ayurveda
- FR: Naturopathie & Ayurveda

**Nav: retreats**  `DRAFT`
- EN: Retreats
- FR: Retraites

**Nav: events**  `DRAFT`
- EN: Events
- FR: Événements

**Nav: library**  `DRAFT`
- EN: Digital Library
- FR: Bibliothèque

**Language switcher**  `REAL`
- EN: EN / FR
- FR: EN / FR

**Primary button (everywhere)**  `DRAFT`
- EN: Book a Session
- FR: Réserver une séance

Link: `https://victorianosenko.clinicsense.com/book/` (new tab)  `REAL`

**Shop (hidden page) nav label**  `DRAFT`
- EN: Shop
- FR: Boutique

### Footer

**Explore (column title)**  `DRAFT`
- EN: Explore
- FR: Explorer

**Connect (column title)**  `DRAFT`
- EN: Connect
- FR: Nous joindre

**Footer name**  `REAL`
- EN: Aspring Health Center
- FR: Aspring Health Center

**Practice description (one line)**  `NEW / FR-NEW`
- EN: Massage therapy, naturopathy and Ayurvedic care in Plateau-Mont-Royal, Montréal.
- FR: Massothérapie, naturopathie et soins ayurvédiques sur le Plateau-Mont-Royal, à Montréal.

**Contact block** `REAL` (confirm in FACTS.md)
- Address: 415 Boul St-Joseph E, Montréal, QC
- Phone: +1 438 498 8415
- Email: aspringhealthcenter@gmail.com
- Hours EN: Mon – Sun, 9 am – 9 pm ET
- Hours FR: Lun – Dim, 9 h – 21 h HE
- Instagram: https://www.instagram.com/aspringhealthcenter/
- Facebook: https://www.facebook.com/people/Aspring-Health-Center/61573919432419/

> ⚠ The mockup footer said "Tue – Sat, by appointment". Replaced by the real hours.

**Newsletter title**  `DRAFT`
- EN: Newsletter
- FR: Infolettre

**Newsletter text**  `DRAFT`
- EN: Seasonal practices, new retreats and the occasional recipe. Once a month, never more.
- FR: Pratiques saisonnières, nouvelles retraites et une recette à l’occasion. Une fois par mois, jamais plus.

**Newsletter button**  `DRAFT`
- EN: Join
- FR: S’abonner

**Newsletter thank-you**  `DRAFT`
- EN: Thank you — you are on the list.
- FR: Merci — vous êtes inscrit.

**Legal line**  `DRAFT`
- EN: RMT receipts provided · Privacy policy
- FR: Reçus de massothérapeute (MA) fournis · Politique de confidentialité

> ⚠ "RMT receipts provided" is a claim to verify (see open issues). Privacy policy page is needed.

**Copyright**  `NEW`
- EN: © 2026 Aspring Health Center
- FR: © 2026 Aspring Health Center

### Form labels (all forms)

**Name**  `DRAFT`
- EN: Your name
- FR: Votre nom

**Email**  `DRAFT`
- EN: Email address
- FR: Adresse courriel

**Message**  `DRAFT`
- EN: What are you hoping for?
- FR: Qu’espérez-vous trouver ?

**Send**  `DRAFT`
- EN: Send inquiry
- FR: Envoyer la demande

**Phone (retreat form)**  `NEW / FR-NEW`
- EN: Phone (optional)
- FR: Téléphone (facultatif)

**Which retreat (retreat form)**  `NEW / FR-NEW`
- EN: Which retreat are you interested in?
- FR: Quelle retraite vous intéresse ?

## 1. Home

### Hero

**Label (kicker)**  `DRAFT`
- EN: Plateau-Mont-Royal, Montréal
- FR: Plateau-Mont-Royal, Montréal

**H1 line 1**  `DRAFT`
- EN: Come home
- FR: Revenir

**H1 line 2 (italic, accent)**  `DRAFT`
- EN: to your body.
- FR: habiter son corps.

**Lead paragraph**  `DRAFT, FACT`
- EN: I'm Victoria. For more than fifteen years, people have come to me exhausted, guarded, living a little outside of themselves — and left breathing differently. Massage, naturopathy, craniosacral therapy and Ayurveda are my tools. Deep restoration is the work.
- FR: Je suis Victoria. Depuis plus de quinze ans, des gens arrivent chez moi épuisés, sur leurs gardes, un peu à côté d’eux-mêmes — et repartent en respirant autrement. La massothérapie, la naturopathie, la thérapie craniosacrale et l’Ayurveda sont mes outils. La restauration profonde est le travail.

> ⚠ "For more than fifteen years" conflicts with the approved email ("nine years") and the old site. Fill the number from FACTS.md.

Buttons: primary = Book a Session (above). Secondary:

**Secondary button**  `DRAFT`
- EN: Explore the work
- FR: Découvrir la pratique

### Stats band

**Stat 1**  `DRAFT, FACT`
- EN: 15+: Years in practice
- FR: 15+ : Années de pratique

**Stat 2**  `DRAFT, FACT`
- EN: 4: Healing modalities
- FR: 4 : Approches thérapeutiques

**Stat 3**  `DRAFT, FACT`
- EN: RMT: Insurance receipts
- FR: RMT : Reçus d’assurance

> ⚠ 15+ years, "4 modalities" and "RMT insurance receipts" are unverified claims. Use FACTS.md.

### Philosophy

**Label**  `DRAFT`
- EN: My philosophy
- FR: Ma philosophie

**Heading (H2)**  `DRAFT`
- EN: The body heals when it finally feels safe enough to.
- FR: Le corps guérit lorsqu’il se sent enfin en sécurité.

**Paragraph 1**  `DRAFT`
- EN: Most people arrive holding something: a shoulder that never softens, sleep that never deepens, digestion that has been off for years. I don't treat those as separate problems. They are usually one nervous system asking for a different pace.
- FR: La plupart des gens arrivent en portant quelque chose : une épaule qui ne se relâche jamais, un sommeil qui ne s’approfondit plus, une digestion difficile depuis des années. Je ne traite pas ces éléments séparément. C’est généralement un seul système nerveux qui demande un autre rythme.

**Paragraph 2**  `DRAFT`
- EN: So we begin slowly. I read the tissue, the breath, the pulse, the story you tell about your days. Then we choose the route — hands-on work to release what is held, herbs and food to rebuild what is depleted, craniosacral work for what needs stillness rather than pressure.
- FR: Nous commençons donc lentement. J’écoute les tissus, le souffle, le pouls, et le récit que vous faites de vos journées. Ensuite nous choisissons la voie : le travail manuel pour relâcher, les plantes et l’alimentation pour reconstruire, le craniosacral pour ce qui demande de l’immobilité plutôt que de la pression.

**Pull quote**  `DRAFT`
- EN: I am not here to fix you. I am here to give your body the conditions it has been waiting for.
- FR: Je ne suis pas là pour vous réparer. Je suis là pour offrir à votre corps les conditions qu’il attend depuis longtemps.

### Credentials & training

**Title**  `DRAFT`
- EN: Credentials & training
- FR: Formations et titres

**Chip 1**  `DRAFT, FACT`
- EN: Registered Massage Therapist (RMT)
- FR: Massothérapeute agréée (RMT)

**Chip 2**  `DRAFT, FACT`
- EN: Naturopath
- FR: Naturopathe

**Chip 3**  `DRAFT, FACT`
- EN: Craniosacral Therapist
- FR: Thérapeute craniosacrale

**Chip 4**  `DRAFT, FACT`
- EN: Ayurvedic Practitioner
- FR: Praticienne en Ayurveda

**Chip 5**  `DRAFT, FACT`
- EN: 15+ years in clinical practice
- FR: Plus de 15 ans de pratique clinique

> ⚠ Chip 5 (15+ years in clinical practice) needs the real number. Chips 1–4 match the credentials in the approved email (RMT, naturopath, craniosacral, Ayurvedic practitioner).

### Featured services (3 cards)

**Section title**  `DRAFT`
- EN: Where we can begin
- FR: Par où commencer

**Section lede**  `DRAFT`
- EN: Three doors into the same work. Most clients move between them over time, and I will tell you honestly which one you need first.
- FR: Trois portes vers le même travail. La plupart des clients passent de l’une à l’autre au fil du temps, et je vous dirai honnêtement laquelle vient en premier.

**Card 1 title**  `DRAFT`
- EN: Massage Therapy
- FR: Massothérapie

**Card 1 text**  `DRAFT`
- EN: Therapeutic, deep tissue, prenatal and craniosacral sessions. RMT receipts for insurance.
- FR: Séances thérapeutiques, tissus profonds, prénatales et craniosacrales. Reçus RMT pour vos assurances.

**Card 1 link**  `DRAFT`
- EN: See sessions & pricing
- FR: Voir séances et tarifs

**Card 2 title**  `DRAFT`
- EN: Naturopathy & Ayurveda
- FR: Naturopathie & Ayurveda

**Card 2 text**  `DRAFT`
- EN: Root-cause consultations, herbal protocols, seasonal Ayurvedic guidance and nutrition.
- FR: Consultations en profondeur, protocoles de plantes, conseils ayurvédiques saisonniers et nutrition.

**Card 2 link**  `DRAFT`
- EN: See consultations
- FR: Voir les consultations

**Card 3 title**  `DRAFT`
- EN: Retreats & Events
- FR: Retraites & événements

**Card 3 text**  `DRAFT`
- EN: Small-group immersions and workshops for people who want to go deeper than an hour.
- FR: Immersions en petits groupes et ateliers, pour aller plus loin qu’une heure sur la table.

**Card 3 link**  `DRAFT`
- EN: See what is coming
- FR: Voir la programmation

> ⚠ Card 1 text mentions "prenatal" sessions, which ClinicSense does not list. Adjust to the real services.

### Testimonials

**Title**  `DRAFT`
- EN: In their words
- FR: Témoignages

**Quote 1**  `PLACEHOLDER`
- EN: I came in for my lower back and left with the first full night of sleep I had had in months. Victoria works with the whole person, not the complaint.
- FR: Je suis venue pour le bas du dos et je suis repartie avec ma première vraie nuit de sommeil en plusieurs mois. Victoria travaille avec la personne entière, pas avec le symptôme.

**Attribution 1**  `PLACEHOLDER`
- EN: Marie-Claude L. · Montréal
- FR: Marie-Claude L. · Montréal

**Quote 2**  `PLACEHOLDER`
- EN: She found the thread between my digestion and my stress in one consultation. The herbal protocol changed my winter.
- FR: Elle a fait le lien entre ma digestion et mon stress en une seule consultation. Le protocole de plantes a changé mon hiver.

**Attribution 2**  `PLACEHOLDER`
- EN: Daniel R. · Mile End
- FR: Daniel R. · Mile End

**Quote 3**  `PLACEHOLDER`
- EN: The craniosacral sessions did something I cannot quite explain. My body finally stopped bracing.
- FR: Les séances craniosacrales ont fait quelque chose que je n’arrive pas à expliquer. Mon corps a enfin arrêté de se contracter.

**Attribution 3**  `PLACEHOLDER`
- EN: Sophie B. · Outremont
- FR: Sophie B. · Outremont

> ⚠ Invented reviews. Replace with real Google reviews.

### Closing call to action

**Heading**  `DRAFT`
- EN: Ready to begin?
- FR: Prêt à commencer ?

**Text**  `DRAFT`
- EN: Sessions are booked online and confirmed by email. If you are unsure which one is right, book an initial consultation and we will decide together.
- FR: Les séances se réservent en ligne et sont confirmées par courriel. Si vous hésitez, réservez une première consultation et nous choisirons ensemble.

## 2. Massage Therapy

**Label**  `DRAFT`
- EN: Registered Massage Therapy
- FR: Massothérapie agréée

**H1**  `DRAFT`
- EN: Hands-on work for a body that has been holding on too long.
- FR: Un travail manuel pour un corps qui retient depuis trop longtemps.

**Lead paragraph**  `DRAFT`
- EN: Every session begins with a short assessment: where it hurts, how you sleep, what your days ask of you. Pressure, pace and technique are chosen from there — never from a menu.
- FR: Chaque séance débute par une courte évaluation : où ça fait mal, comment vous dormez, ce que vos journées exigent de vous. La pression, le rythme et la technique découlent de là — jamais d’un menu.

### Sessions and pricing: REAL, from ClinicSense

Prices in CAD, as listed in ClinicSense. Durations/prices render as a repeating list (connectable to a CMS collection). Page mapping below is a proposal.

**On this page (7 services):**

**Functional Health Massage**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Massage santé fonctionnel
- Durations / prices: 60 min $100 · 75 min $120 · 90 min $140 · 120 min $180
- Card blurb EN: A full-body treatment tailored to you, combining Swedish, deep tissue and aromatherapy techniques.  `NEW`
- Card blurb FR: Un soin complet du corps, adapté à vos besoins, mêlant techniques suédoises, tissus profonds et aromathérapie.  `FR-NEW`
- Website description EN (softened from Victoria's text): A full-body massage shaped around what your body needs on the day. Within one session I may combine techniques such as Swedish, deep tissue, aromatherapy and maderotherapy. Afterwards we talk through how you feel, and I suggest aftercare: stretches, hydration and, if it would help, follow-up sessions. For a full programme I suggest a series of about ten sessions, with two to three days between the first six to eight.  `REAL, softened`
- Website description FR: Un massage complet du corps, façonné selon ce dont votre corps a besoin ce jour-là. Au cours d'une même séance, je peux associer des techniques comme le massage suédois, les tissus profonds, l'aromathérapie et la maderothérapie. Nous échangeons ensuite sur vos sensations, et je vous propose des conseils de suivi : étirements, hydratation et, si cela vous aide, d'autres séances. Pour un programme complet, je suggère une série d'environ dix séances, espacées de deux à trois jours pour les six à huit premières.  `FR-NEW`

**Deep tissue massage**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Massage des tissus profonds
- Durations / prices: 75 min $120 · 90 min $150
- Card blurb EN: Slow, firm pressure for the deeper muscle layers and long-held tension in the neck, shoulders, back and legs.  `NEW`
- Card blurb FR: Une pression lente et ferme pour les couches musculaires profondes et les tensions installées : cou, épaules, dos et jambes.  `FR-NEW`
- Website description EN (softened from Victoria's text): Slow, deliberate strokes and firm pressure reach the deeper layers of muscle and connective tissue. This session suits long-standing tightness in the neck, shoulders, upper back or legs, muscle stiffness, and the strain that follows sport. Many clients also notice easier movement and a general sense of release afterwards.  `REAL, softened`
- Website description FR: Des mouvements lents et une pression ferme atteignent les couches plus profondes des muscles et du tissu conjonctif. Cette séance convient aux tensions installées dans la nuque, les épaules, le haut du dos ou les jambes, à la raideur musculaire et à la fatigue liée au sport. Beaucoup de clients ressentent aussi plus de liberté de mouvement et une impression générale de détente ensuite.  `FR-NEW`

**First Visit Health Massage**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Massage santé, première visite
- Durations / prices: 60 min $79 · 75 min $95 · 90 min $120
- Card blurb EN: Your first session: a short consultation, then a massage tailored to what you need.  `NEW`
- Card blurb FR: Votre première séance : un court échange, puis un massage adapté à vos besoins.  `FR-NEW`
- Website description EN (softened from Victoria's text): Your first session with me. We begin with a short conversation of about five minutes about your health history, any concerns and the places where you feel tension, so I can tailor the treatment to you. The massage draws on techniques such as Swedish, deep tissue and aromatherapy. Afterwards we talk about how you feel, and I suggest aftercare and help you plan future visits. Many clients find that coming about twice a month supports their wellness goals. Ask me anything beforehand: your comfort comes first.  `REAL, softened`
- Website description FR: Votre première séance avec moi. Nous commençons par un court échange d'environ cinq minutes sur votre historique de santé, vos préoccupations et les endroits où vous ressentez des tensions, afin d'adapter le soin à vos besoins. Le massage fait appel à des techniques comme le massage suédois, les tissus profonds et l'aromathérapie. Ensuite, nous parlons de vos sensations, je vous propose des conseils de suivi et je vous aide à planifier vos prochaines visites. Beaucoup de clients trouvent qu'une visite environ deux fois par mois soutient leurs objectifs de bien-être. N'hésitez pas à me poser vos questions : votre confort passe avant tout.  `FR-NEW`

**European Sculpting Facial Massage**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Massage sculptant du visage (européen)
- Durations / prices: 60 min $100
- Card blurb EN: A facial massage for deep relaxation, circulation and a natural lift, without invasive methods.  `NEW`
- Card blurb FR: Un massage du visage pour la détente profonde, la circulation et un effet liftant naturel, sans méthode invasive.  `FR-NEW`
- Website description EN (softened from Victoria's text): A facial massage that combines deep muscle relaxation, circulation and natural lifting techniques, with no invasive methods. It is designed to ease tension in the face and leave the skin looking fresh and relaxed.  `REAL, softened`
- Website description FR: Un massage du visage qui associe relaxation musculaire profonde, circulation et techniques de lissage et de lifting naturel, sans méthode invasive. Il vise à relâcher les tensions du visage et à laisser la peau fraîche et détendue.  `FR-NEW`

**Reiki Healing Session**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Séance de Reiki
- Durations / prices: 60 min $100
- Card blurb EN: Gentle energy work to support relaxation and balance.  `NEW`
- Card blurb FR: Un travail énergétique doux pour favoriser la détente et l'équilibre.  `FR-NEW`
- Website description EN (softened from Victoria's text): A gentle energy session offered to support relaxation, balance and a sense of well-being in body, mind and spirit.  `REAL, softened`
- Website description FR: Une séance d'énergie douce proposée pour favoriser la détente, l'équilibre et le bien-être du corps, de l'esprit et de l'âme.  `FR-NEW`

**Anti-Cortisol Massage**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Massage anti-cortisol
- Durations / prices: 60 min $100
- Card blurb EN: Moderate-pressure Swedish and myofascial massage with guided breathing, aromatherapy and an Ayurvedic tea ritual, designed for stress.  `NEW`
- Card blurb FR: Massage suédois et myofascial à pression modérée, respiration guidée, aromathérapie et rituel de thé ayurvédique, pour apaiser le stress.  `FR-NEW`
- Website description EN (softened from Victoria's text): A session designed for people living with ongoing stress. It combines moderate-pressure Swedish and myofascial massage for the shoulders, back, neck and hips; diaphragm release with guided breathing; a scalp and foot ritual; lavender and bergamot aromatherapy; and an Ayurvedic tea ritual afterwards. Many clients leave feeling calmer and sleep more easily, and regular sessions, about every two to four weeks, help them keep that calm. To prepare, hydrate, eat lightly, avoid alcohol and caffeine, and arrive five to ten minutes early. Afterwards, drink warm water, rest, and avoid intense exercise for 12 to 24 hours.  `REAL, softened`
- Website description FR: Une séance conçue pour les personnes qui vivent avec un stress constant. Elle associe un massage suédois et myofascial à pression modérée pour les épaules, le dos, la nuque et les hanches ; un relâchement du diaphragme avec respiration guidée ; un rituel du cuir chevelu et des pieds ; l'aromathérapie à la lavande et à la bergamote ; et un rituel de thé ayurvédique ensuite. Beaucoup de clients repartent plus calmes et dorment plus facilement ; des séances régulières, environ toutes les deux à quatre semaines, les aident à garder ce calme. Pour vous préparer : hydratez-vous, mangez léger, évitez l'alcool et la caféine, et arrivez cinq à dix minutes à l'avance. Après la séance, buvez de l'eau chaude, reposez-vous et évitez les efforts intenses pendant 12 à 24 heures.  `FR-NEW`

**Professional Neck Osteochondrosis Therapy session**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Séance de thérapie pour la nuque (ostéochondrose)
- Durations / prices: 60 min $100
- Card blurb EN: A focused 60-minute session for chronic neck pain, stiffness and tension.  `NEW`
- Card blurb FR: Une séance ciblée de 60 minutes pour les douleurs, raideurs et tensions chroniques de la nuque.  `FR-NEW`
- Website description EN (softened from Victoria's text): A focused 60-minute session for chronic neck tension, stiffness, and the headaches or numbness that can come with them. Using manual techniques, I work on the muscles and tissues of the neck and shoulders, with the aim of easing tension and supporting circulation. The session is tailored to your situation, and many clients notice a difference over a few sessions. It is a targeted treatment rather than a general massage. If you have numbness or symptoms that persist, please also speak with your doctor.  `REAL, softened`
- Website description FR: Une séance ciblée de 60 minutes pour les tensions chroniques de la nuque, la raideur, et les maux de tête ou engourdissements qui peuvent les accompagner. Avec des techniques manuelles, je travaille les muscles et les tissus de la nuque et des épaules, dans le but de relâcher les tensions et de soutenir la circulation. La séance est adaptée à votre situation, et beaucoup de clients remarquent une différence en quelques séances. C'est un soin ciblé plutôt qu'un massage général. Si vous avez des engourdissements ou des symptômes qui persistent, parlez-en aussi à votre médecin.  `FR-NEW`

> ⚠ Website descriptions are softened versions of Victoria's ClinicSense text (no "proven", no percentages, no "eliminate/break down deposits", no "lasting results", no named second practitioner). Her original wording is kept only in `content/source/clinicsense-services.json`. Use these, not the originals.

**Insurance label**  `DRAFT`
- EN: RMT
- FR: RMT

**Insurance title**  `DRAFT`
- EN: Insurance receipts provided
- FR: Reçus d’assurance fournis

**Insurance text**  `DRAFT, FACT`
- EN: As a Registered Massage Therapist, I issue receipts accepted by most Québec extended-health plans.
- FR: À titre de massothérapeute agréée, je remets des reçus acceptés par la plupart des régimes d’assurance collective au Québec.

**Insurance bullet 1**  `DRAFT, FACT`
- EN: Receipt emailed after every session
- FR: Reçu envoyé par courriel après chaque séance

**Insurance bullet 2**  `DRAFT, FACT`
- EN: Accepted by most private insurers
- FR: Accepté par la plupart des assureurs privés

**Insurance bullet 3**  `DRAFT, FACT`
- EN: Direct billing not required
- FR: Aucune facturation directe requise

> ⚠ Unverified: receipt acceptance, insurers, "direct billing not required".

**Price note**  `DRAFT, FACT`
- EN: Taxes included. 24-hour cancellation policy. Packages of five sessions available on request.
- FR: Taxes incluses. Annulation 24 h à l’avance. Forfaits de cinq séances offerts sur demande.

> ⚠ "Taxes included", the cancellation policy and "packages of five" are not on ClinicSense. Confirm or remove.

**Booking heading**  `DRAFT`
- EN: Book your session
- FR: Réservez votre séance

**Booking text**  `DRAFT`
- EN: Online booking shows my live availability. Choose a time, tell me briefly what brings you in, and you will receive a confirmation by email.
- FR: La réservation en ligne affiche mes disponibilités réelles. Choisissez un moment, indiquez brièvement ce qui vous amène, et vous recevrez une confirmation par courriel.

**Booking button**  `DRAFT`
- EN: Open the booking calendar
- FR: Ouvrir le calendrier

**Booking note**  `DRAFT, FACT`
- EN: Evenings and Saturdays available
- FR: Soirs et samedis disponibles

> ⚠ "Evenings and Saturdays available" must match the real hours.

Phone beside the button: +1 438 498 8415  `REAL`

## 3. Naturopathy & Ayurveda

**Label**  `DRAFT`
- EN: Naturopathy & Ayurveda
- FR: Naturopathie & Ayurveda

**H1**  `DRAFT`
- EN: Care that looks for the cause, not only the symptom.
- FR: Des soins qui cherchent la cause, pas seulement le symptôme.

**Lead paragraph**  `DRAFT`
- EN: Naturopathy gives me the assessment tools; Ayurveda gives me a framework for constitution and season. Together they let us build something you can actually live with — food, herbs, rhythm, rest.
- FR: La naturopathie me donne les outils d’évaluation ; l’Ayurveda, un cadre pour la constitution et les saisons. Ensemble, elles permettent de bâtir quelque chose de vivable : alimentation, plantes, rythme, repos.

### Services: REAL, from ClinicSense (5 services)

**Naturopathy**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Naturopathie
- Durations / prices: 60 min $100
- Card blurb EN: Holistic care blending Ayurveda, yoga therapy and personalized nutrition, working on root causes.  `NEW`
- Card blurb FR: Une approche holistique alliant ayurvéda, yoga-thérapie et nutrition personnalisée, centrée sur les causes profondes.  `FR-NEW`
- Website description EN (softened from Victoria's text): Holistic care that blends naturopathy, Ayurveda, yoga therapy and personalized nutrition. We look at the root causes of how you feel and use natural remedies and therapeutic practices to support balance and vitality, so you can reconnect with your body's own capacity to heal.  `REAL, softened`
- Website description FR: Des soins holistiques qui allient naturopathie, ayurvéda, yoga-thérapie et nutrition personnalisée. Nous cherchons les causes profondes de ce que vous ressentez et nous utilisons des remèdes naturels et des pratiques thérapeutiques pour soutenir l'équilibre et la vitalité, afin que vous renouiez avec la capacité de votre corps à se régénérer.  `FR-NEW`

**Personalised Ayurvedic Menu**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Menu ayurvédique personnalisé
- Durations / prices: 60 min $100
- Card blurb EN: An online consultation: a personalized Ayurvedic nutrition and lifestyle plan based on your dosha.  `NEW`
- Card blurb FR: Une consultation en ligne : un plan alimentaire et de style de vie ayurvédique personnalisé selon votre dosha.  `FR-NEW`
- Website description EN (softened from Victoria's text): An online consultation that gives you a personalized Ayurvedic nutrition and lifestyle plan based on your dosha (body type). It includes a food list tailored to balance your dosha, morning and evening rituals for vitality, and easy, natural detox suggestions. This is not a diet: it is a way of eating and living that follows your body's natural rhythm.  `REAL, softened`
- Website description FR: Une consultation en ligne qui vous remet un plan alimentaire et de style de vie ayurvédique personnalisé, selon votre dosha (type corporel). Il comprend une liste d'aliments adaptée pour équilibrer votre dosha, des rituels du matin et du soir pour la vitalité, et des suggestions de détox simples et naturelles. Ce n'est pas un régime : c'est une façon de manger et de vivre qui suit le rythme naturel de votre corps.  `FR-NEW`

**CranioSacral therapy**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Thérapie crânio-sacrée
- Durations / prices: 60 min $100
- Card blurb EN: A gentle, non-invasive therapy that supports the body's natural healing processes and deep relaxation.  `NEW`
- Card blurb FR: Une thérapie douce et non invasive qui soutient les processus naturels de guérison du corps et favorise une relaxation profonde.  `FR-NEW`
- Website description EN (softened from Victoria's text): A gentle, non-invasive therapy that supports the body's natural healing processes. Craniosacral therapy was developed by Dr. John E. Upledger, an osteopathic physician, who explored the craniosacral system: the membranes and cerebrospinal fluid surrounding the brain and spinal cord. With light touch, I look for areas of restriction and encourage them to release, working toward deep relaxation and ease. Clients often come for tension and stress, or to feel more balanced. A session is calm and supportive, and always tailored to you.  `REAL, softened`
- Website description FR: Une thérapie douce et non invasive qui soutient les processus naturels de guérison du corps. La thérapie crânio-sacrée a été développée par le Dr John E. Upledger, médecin ostéopathe, qui a exploré le système crânio-sacré : les membranes et le liquide céphalo-rachidien qui entourent le cerveau et la moelle épinière. Par un toucher léger, je repère les zones de restriction et j'encourage leur relâchement, en visant une relaxation profonde et un sentiment d'aisance. Les clients viennent souvent pour des tensions et du stress, ou pour retrouver plus d'équilibre. La séance est calme et rassurante, et toujours adaptée à vous.  `FR-NEW`

**Shirodhara session**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Séance de Shirodhara
- Durations / prices: 75 min $180
- Card blurb EN: A continuous stream of warm herbal oil over the forehead for deep relaxation and calm.  `NEW`
- Card blurb FR: Un filet continu d'huile chaude aux herbes sur le front pour une relaxation profonde et le calme.  `FR-NEW`
- Website description EN (softened from Victoria's text): An ancient Ayurvedic treatment in which a continuous stream of warm herbal oil is gently poured over the forehead. The name comes from the Sanskrit shiro (head) and dhara (flow). You lie comfortably on the table while the oil flows for about 30 to 45 minutes, which many people find deeply meditative. Shirodhara is traditionally used to support relaxation, sleep, mental clarity and emotional balance, and the herbal oil blend is chosen to suit your constitution (dosha).  `REAL, softened`
- Website description FR: Un soin ayurvédique ancestral dans lequel un filet continu d'huile chaude aux herbes est doucement versé sur le front. Le nom vient du sanskrit shiro (tête) et dhara (flux). Vous êtes installé confortablement sur la table pendant que l'huile s'écoule, environ 30 à 45 minutes, une expérience que beaucoup trouvent profondément méditative. Le Shirodhara est traditionnellement utilisé pour soutenir la détente, le sommeil, la clarté mentale et l'équilibre émotionnel, et le mélange d'huiles aux herbes est choisi selon votre constitution (dosha).  `FR-NEW`

**Monsalada massage**  `REAL (name, durations, prices)` · FR name `FR-NEW`
- FR name: Massage Monsalada
- Durations / prices: 120 min $200
- Card blurb EN: A method of feminine body therapy combining guided meditation, craniosacral work, Ayurvedic hot-oil massage and a coaching conversation.  `NEW`
- Card blurb FR: Une méthode de thérapie corporelle féminine : méditation guidée, thérapie crânio-sacrée, massage ayurvédique à l'huile chaude et échange de coaching.  `FR-NEW`
- Website description EN (softened from Victoria's text): Monsalada is a method of feminine body therapy, offered as a holistic and deeply personal experience for women. It is built on the idea that body and mind are indivisible, and it works as a practical tool for physical and emotional release. A session includes a foot-cleansing ritual, guided meditation, craniosacral therapy, an Ayurvedic hot-oil massage and a coaching conversation. I suggest a series of at least three sessions, about three weeks apart.  `REAL, softened`
- Website description FR: Monsalada est une méthode de thérapie corporelle féminine, proposée comme une expérience holistique et profondément personnelle pour les femmes. Elle repose sur l'idée que le corps et l'esprit sont indissociables, et elle sert d'outil pratique de détente physique et émotionnelle. Une séance comprend un rituel de purification des pieds, une méditation guidée, de la thérapie crânio-sacrée, un massage ayurvédique à l'huile chaude et un échange de coaching. Je suggère une série d'au moins trois séances, espacées d'environ trois semaines.  `FR-NEW`

### Client draft: the four consultation types

> ⚠ The mockup describes four consultation types and a process (75-minute assessment, lab review, written protocol, check-ins at four and eight weeks). ClinicSense lists only *Naturopathy* (60 min, $100) and the *Personalised Ayurvedic Menu*. Treat the process as `DRAFT` until Victoria confirms what she actually offers.

**"What it brings you" label**  `DRAFT`
- EN: What it brings you
- FR: Ce que cela vous apporte

**Service 1 name**  `DRAFT`
- EN: Naturopathic Consultation
- FR: Consultation naturopathique

**Service 1 text**  `DRAFT`
- EN: A long first appointment covering history, digestion, sleep, cycle, stress and energy. We map patterns, then build a protocol in stages so nothing is overwhelming.
- FR: Un premier rendez-vous long : antécédents, digestion, sommeil, cycle, stress et énergie. Nous dégageons les schémas, puis construisons un protocole par étapes.

**Service 1 benefit 1**  `DRAFT`
- EN: A clear picture of what is driving your symptoms
- FR: Une vision claire de ce qui alimente vos symptômes

**Service 1 benefit 2**  `DRAFT`
- EN: A staged plan for food, supplements and habits
- FR: Un plan progressif : alimentation, suppléments, habitudes

**Service 1 benefit 3**  `DRAFT`
- EN: Follow-up adjustments as your body responds
- FR: Des ajustements de suivi selon vos réactions

**Service 2 name**  `DRAFT`
- EN: Ayurvedic Assessment
- FR: Évaluation ayurvédique

**Service 2 text**  `DRAFT`
- EN: Pulse and constitution reading to identify your dosha balance and where it has drifted. From there, seasonal recommendations for eating, sleeping and moving.
- FR: Lecture du pouls et de la constitution pour situer votre équilibre doshique et son déséquilibre. Suivent des recommandations saisonnières pour manger, dormir et bouger.

**Service 2 benefit 1**  `DRAFT`
- EN: Your constitutional baseline in plain language
- FR: Votre profil constitutionnel en mots simples

**Service 2 benefit 2**  `DRAFT`
- EN: Seasonal routines suited to Montréal
- FR: Des routines saisonnières adaptées à Montréal

**Service 2 benefit 3**  `DRAFT`
- EN: Practices that steady mood and digestion
- FR: Des pratiques qui stabilisent humeur et digestion

**Service 3 name**  `DRAFT`
- EN: Herbal & Nutritional Protocols
- FR: Protocoles de plantes et nutrition

**Service 3 text**  `DRAFT`
- EN: Targeted formulas and food strategy for digestion, hormonal balance, immunity, sleep and depletion. Prepared in small batches, adjusted at each visit.
- FR: Formules ciblées et stratégie alimentaire pour la digestion, l’équilibre hormonal, l’immunité, le sommeil et l’épuisement. Préparées en petites quantités, ajustées à chaque visite.

**Service 3 benefit 1**  `DRAFT`
- EN: Formulas matched to you, not a category
- FR: Des formules adaptées à vous, pas à une catégorie

**Service 3 benefit 2**  `DRAFT`
- EN: Realistic food guidance, no elimination for its own sake
- FR: Des conseils alimentaires réalistes, sans exclusion inutile

**Service 3 benefit 3**  `DRAFT`
- EN: Clear dosing and duration
- FR: Un dosage et une durée clairs

**Service 4 name**  `DRAFT`
- EN: Nervous System Recovery
- FR: Récupération du système nerveux

**Service 4 text**  `DRAFT`
- EN: For burnout, chronic stress and long recovery. Combines naturopathic support with craniosacral sessions and Ayurvedic daily rhythm.
- FR: Pour l’épuisement, le stress chronique et les convalescences longues. Combine le soutien naturopathique, les séances craniosacrales et le rythme quotidien ayurvédique.

**Service 4 benefit 1**  `DRAFT`
- EN: Deeper, more continuous sleep
- FR: Un sommeil plus profond et continu

**Service 4 benefit 2**  `DRAFT`
- EN: Steadier energy through the day
- FR: Une énergie plus stable dans la journée

**Service 4 benefit 3**  `DRAFT`
- EN: Better tolerance for stress
- FR: Une meilleure tolérance au stress

### Consultation process (DRAFT)

**Title**  `DRAFT`
- EN: The consultation process
- FR: Le déroulement d’une consultation

**Lead**  `DRAFT`
- EN: Four steps, usually over three months. You leave every appointment knowing exactly what to do next.
- FR: Quatre étapes, généralement sur trois mois. Vous quittez chaque rendez-vous en sachant exactement quoi faire ensuite.

**Step 1 number**  `DRAFT`
- EN: One
- FR: Un

**Step 1 title**  `DRAFT`
- EN: Intake
- FR: Questionnaire

**Step 1 text**  `DRAFT`
- EN: A detailed questionnaire before we meet, so our time together is spent on you rather than paperwork.
- FR: Un questionnaire détaillé avant la rencontre, pour consacrer notre temps à vous plutôt qu’à la paperasse.

**Step 2 number**  `DRAFT`
- EN: Two
- FR: Deux

**Step 2 title**  `DRAFT`
- EN: Assessment
- FR: Évaluation

**Step 2 text**  `DRAFT`
- EN: 75 minutes: history, pulse and constitution reading, and where relevant, lab review.
- FR: 75 minutes : antécédents, lecture du pouls et de la constitution, et revue des analyses le cas échéant.

**Step 3 number**  `DRAFT`
- EN: Three
- FR: Trois

**Step 3 title**  `DRAFT`
- EN: Protocol
- FR: Protocole

**Step 3 text**  `DRAFT`
- EN: A written plan within a week — food, herbs, supplements, routine — staged over the coming weeks.
- FR: Un plan écrit dans la semaine — alimentation, plantes, suppléments, routine — échelonné sur les semaines à venir.

**Step 4 number**  `DRAFT`
- EN: Four
- FR: Quatre

**Step 4 title**  `DRAFT`
- EN: Follow-up
- FR: Suivi

**Step 4 text**  `DRAFT`
- EN: Two check-ins at four and eight weeks to adjust dosing and refine what is working.
- FR: Deux suivis, à quatre et huit semaines, pour ajuster les doses et affiner ce qui fonctionne.

### Licenses and certifications (PLACEHOLDER)

**Title**  `DRAFT`
- EN: Licenses & certifications
- FR: Titres et certifications

**Entry 1 name**  `PLACEHOLDER`
- EN: Registered Massage Therapist (RMT)
- FR: Massothérapeute agréée (RMT)

**Entry 1 issuer**  `PLACEHOLDER`
- EN: Fédération québécoise des massothérapeutes
- FR: Fédération québécoise des massothérapeutes

**Entry 1 status**  `PLACEHOLDER`
- EN: Active
- FR: Actif

**Entry 2 name**  `PLACEHOLDER`
- EN: Diploma in Naturopathy
- FR: Diplôme en naturopathie

**Entry 2 issuer**  `PLACEHOLDER`
- EN: Accredited naturopathic college
- FR: Collège de naturopathie accrédité

**Entry 2 status**  `PLACEHOLDER`
- EN: Certified
- FR: Certifiée

**Entry 3 name**  `PLACEHOLDER`
- EN: Craniosacral Therapy, Levels I–IV
- FR: Thérapie craniosacrale, niveaux I à IV

**Entry 3 issuer**  `PLACEHOLDER`
- EN: Upledger-method training
- FR: Formation méthode Upledger

**Entry 3 status**  `PLACEHOLDER`
- EN: Certified
- FR: Certifiée

**Entry 4 name**  `PLACEHOLDER`
- EN: Ayurvedic Practitioner
- FR: Praticienne en Ayurveda

**Entry 4 issuer**  `PLACEHOLDER`
- EN: Ayurvedic institute training
- FR: Formation en institut ayurvédique

**Entry 4 status**  `PLACEHOLDER`
- EN: Certified
- FR: Certifiée

**Entry 5 name**  `PLACEHOLDER`
- EN: Continuing education
- FR: Formation continue

**Entry 5 issuer**  `PLACEHOLDER`
- EN: Annual clinical training since 2010
- FR: Perfectionnement clinique annuel depuis 2010

**Entry 5 status**  `PLACEHOLDER`
- EN: Ongoing
- FR: En cours

> ⚠ Issuing bodies and years are guesses. Needs Victoria's real credentials. The approved email says: craniosacral therapy; Reiki and Tibetan healing traditions under Buddhist masters in Nepal and India; first certified Monsalada practitioner in Canada.

### Related natural products (PLACEHOLDER)

**Title**  `DRAFT`
- EN: Related natural products
- FR: Produits naturels complémentaires

**Lead**  `DRAFT`
- EN: A small, curated shelf — the herbs and oils I actually use in the clinic. Available at your appointment or by request.
- FR: Une petite sélection : les plantes et les huiles que j’utilise réellement en clinique. Disponibles lors de votre rendez-vous ou sur demande.

**Product 1 name**  `PLACEHOLDER`
- EN: Herbal Tea Blends
- FR: Mélanges de tisanes

**Product 1 text**  `PLACEHOLDER`
- EN: Digestive, calming and immune blends, prepared in small batches.
- FR: Mélanges digestifs, apaisants et immunitaires, préparés en petites quantités.

**Product 2 name**  `PLACEHOLDER`
- EN: Ayurvedic Body Oils
- FR: Huiles corporelles ayurvédiques

**Product 2 text**  `PLACEHOLDER`
- EN: Warming and cooling oils for daily self-massage, chosen by constitution.
- FR: Huiles réchauffantes ou rafraîchissantes pour l’auto-massage quotidien, selon la constitution.

**Product 3 name**  `PLACEHOLDER`
- EN: Practitioner Supplements
- FR: Suppléments professionnels

**Product 3 text**  `PLACEHOLDER`
- EN: Professional-grade formulas dispensed only alongside a consultation.
- FR: Formules de qualité professionnelle, remises uniquement avec une consultation.

## 4. Retreats

> ⚠ Everything below is the client's draft. She confirmed the retreats and events in her drafts are the only ones. Dates, places and prices still need her confirmation.

**Label**  `DRAFT`
- EN: Retreats
- FR: Retraites

**H1**  `DRAFT`
- EN: Time away, long enough for something to change.
- FR: Du temps à l’écart, assez longtemps pour que quelque chose change.

**Lead**  `DRAFT`
- EN: An hour on the table can interrupt a pattern. Three days can rewrite it. Retreats are small — eight to twelve people — and built around rest rather than activity.
- FR: Une heure sur la table peut interrompre un schéma. Trois jours peuvent le réécrire. Les retraites sont petites — de huit à douze personnes — et construites autour du repos plutôt que des activités.

**Section title: upcoming**  `DRAFT`
- EN: Upcoming retreats
- FR: Retraites à venir

**Button**  `DRAFT`
- EN: Inquire
- FR: S’informer

**Upcoming 1: Status**  `DRAFT, FACT`
- EN: Registration open
- FR: Inscriptions ouvertes

**Upcoming 1: Places**  `DRAFT, FACT`
- EN: 4 of 12 places left
- FR: 4 places sur 12 restantes

**Upcoming 1: Name**  `DRAFT, FACT`
- EN: Winter Stillness
- FR: Silence d’hiver

**Upcoming 1: Dates**  `DRAFT, FACT`
- EN: February 13–16, 2027
- FR: 13 au 16 février 2027

**Upcoming 1: Location**  `DRAFT, FACT`
- EN: Laurentians, QC
- FR: Laurentides, QC

**Upcoming 1: Description**  `DRAFT, FACT`
- EN: Four days in deep winter: daily bodywork, Ayurvedic meals built for cold season, craniosacral sessions, long unstructured afternoons. For people running on empty.
- FR: Quatre jours au cœur de l’hiver : travail corporel quotidien, repas ayurvédiques pensés pour la saison froide, séances craniosacrales et longs après-midis sans horaire. Pour ceux qui n’ont plus de réserve.

**Upcoming 1: Price**  `DRAFT, FACT`
- EN: From $1,480
- FR: À partir de 1 480 $

**Upcoming 1: included 1**  `DRAFT`
- EN: Three nights, private room
- FR: Trois nuits, chambre privée

**Upcoming 1: included 2**  `DRAFT`
- EN: Two individual treatments
- FR: Deux traitements individuels

**Upcoming 1: included 3**  `DRAFT`
- EN: All meals, Ayurvedic kitchen
- FR: Tous les repas, cuisine ayurvédique

**Upcoming 1: included 4**  `DRAFT`
- EN: Daily breathwork and guided rest
- FR: Respiration et repos guidé chaque jour

**Upcoming 2: Status**  `DRAFT, FACT`
- EN: Early booking
- FR: Réservation anticipée

**Upcoming 2: Places**  `DRAFT, FACT`
- EN: 10 places
- FR: 10 places

**Upcoming 2: Name**  `DRAFT, FACT`
- EN: Spring Reset
- FR: Renouveau du printemps

**Upcoming 2: Dates**  `DRAFT, FACT`
- EN: May 8–11, 2027
- FR: 8 au 11 mai 2027

**Upcoming 2: Location**  `DRAFT, FACT`
- EN: Eastern Townships, QC
- FR: Estrie, QC

**Upcoming 2: Description**  `DRAFT, FACT`
- EN: A seasonal cleanse in the Ayurvedic sense: lighter food, herbal support, walking, and enough sleep to feel the difference. Ends with a personal protocol for the summer.
- FR: Une cure saisonnière au sens ayurvédique : alimentation plus légère, soutien par les plantes, marche, et assez de sommeil pour sentir la différence. Se termine par un protocole personnel pour l’été.

**Upcoming 2: Price**  `DRAFT, FACT`
- EN: From $1,320
- FR: À partir de 1 320 $

**Upcoming 2: included 1**  `DRAFT`
- EN: Three nights, shared or private
- FR: Trois nuits, chambre partagée ou privée

**Upcoming 2: included 2**  `DRAFT`
- EN: Individual naturopathic consultation
- FR: Consultation naturopathique individuelle

**Upcoming 2: included 3**  `DRAFT`
- EN: Seasonal cleanse meals
- FR: Repas de cure saisonnière

**Upcoming 2: included 4**  `DRAFT`
- EN: Take-home protocol
- FR: Protocole à emporter

**Section title: past**  `DRAFT`
- EN: Past retreats
- FR: Retraites passées

**Past 1: Name**  `DRAFT, FACT`
- EN: Autumn Grounding
- FR: Ancrage d’automne

**Past 1: Dates**  `DRAFT, FACT`
- EN: October 2026
- FR: Octobre 2026

**Past 1: Location**  `DRAFT, FACT`
- EN: Charlevoix, QC
- FR: Charlevoix, QC

**Past 1: Description**  `DRAFT, FACT`
- EN: Twelve participants, four days of Abhyanga, forest walks and evening breathwork as the season turned.
- FR: Douze participants, quatre jours d’Abhyanga, de marches en forêt et de respiration en soirée, au tournant de la saison.

**Past 2: Name**  `DRAFT, FACT`
- EN: Summer Breath
- FR: Souffle d’été

**Past 2: Dates**  `DRAFT, FACT`
- EN: July 2026
- FR: Juillet 2026

**Past 2: Location**  `DRAFT, FACT`
- EN: Lanaudière, QC
- FR: Lanaudière, QC

**Past 2: Description**  `DRAFT, FACT`
- EN: A lighter, outdoor-facing weekend: morning practice by the water, bodywork in the afternoon.
- FR: Un week-end plus léger, tourné vers l’extérieur : pratique du matin au bord de l’eau, travail corporel l’après-midi.

**Past 3: Name**  `DRAFT, FACT`
- EN: Winter Stillness I
- FR: Silence d’hiver I

**Past 3: Dates**  `DRAFT, FACT`
- EN: February 2026
- FR: Février 2026

**Past 3: Location**  `DRAFT, FACT`
- EN: Laurentians, QC
- FR: Laurentides, QC

**Past 3: Description**  `DRAFT, FACT`
- EN: The first winter edition, and the reason it now runs every year.
- FR: La première édition hivernale, et la raison pour laquelle elle revient chaque année.

**Inquiry form title**  `DRAFT`
- EN: Ask about a retreat
- FR: Renseignez-vous sur une retraite

**Inquiry form lead**  `DRAFT`
- EN: Tell me which retreat interests you and where you are starting from. I answer every inquiry personally, usually within two days.
- FR: Dites-moi quelle retraite vous intéresse et d’où vous partez. Je réponds personnellement à chaque demande, généralement en deux jours.

**Dropdown option 1**  `DRAFT`
- EN: Winter Stillness — February 2027
- FR: Silence d’hiver — février 2027

**Dropdown option 2**  `DRAFT`
- EN: Spring Reset — May 2027
- FR: Renouveau du printemps — mai 2027

**Dropdown option 3**  `DRAFT`
- EN: A future retreat / join the waitlist
- FR: Une retraite future / liste d’attente

**Thank-you title**  `DRAFT`
- EN: Thank you.
- FR: Merci.

**Thank-you text**  `DRAFT`
- EN: Your inquiry has been sent. I will write back personally within two business days.
- FR: Votre demande a été envoyée. Je vous répondrai personnellement dans les deux jours ouvrables.

## 5. Events

> ⚠ Client draft. Dates carry no year and some are already past (Sep 17). Confirm real events and dates.

**Label**  `DRAFT`
- EN: Workshops & group events
- FR: Ateliers et événements de groupe

**H1**  `DRAFT`
- EN: Smaller gatherings, in the clinic and around Montréal.
- FR: Des rassemblements plus intimes, en clinique et à Montréal.

**Lead**  `DRAFT`
- EN: Evening workshops and short series for people who want to learn the practices rather than only receive them. Most run for eight to sixteen participants.
- FR: Des ateliers en soirée et de courtes séries, pour celles et ceux qui veulent apprendre les pratiques plutôt que seulement les recevoir. La plupart accueillent de huit à seize participants.

**Register button**  `DRAFT`
- EN: Register
- FR: S’inscrire

**Filter chips**  `NEW / FR-NEW`
- EN: All · Workshops · Group Classes · Talks
- FR: Tous · Ateliers · Cours de groupe · Conférences

**Event 1: Month**  `DRAFT, FACT`
- EN: Sep
- FR: Sep

**Event 1: Day**  `DRAFT, FACT`
- EN: 17
- FR: 17

**Event 1: Type**  `DRAFT, FACT`
- EN: Workshop
- FR: Atelier

**Event 1: Time**  `DRAFT, FACT`
- EN: 18:30 – 20:30
- FR: 18 h 30 – 20 h 30

**Event 1: Title**  `DRAFT, FACT`
- EN: Self-Massage for Winter Bodies
- FR: L’auto-massage pour les corps d’hiver

**Event 1: Description**  `DRAFT, FACT`
- EN: Abhyanga technique, oil selection by constitution, and a short daily routine you will actually keep. Oils included.
- FR: Technique d’Abhyanga, choix des huiles selon la constitution et une courte routine quotidienne que vous garderez vraiment. Huiles incluses.

**Event 1: Price**  `DRAFT, FACT`
- EN: $65
- FR: 65 $

**Event 1: Places**  `DRAFT, FACT`
- EN: 6 places left
- FR: 6 places restantes

**Event 2: Month**  `DRAFT, FACT`
- EN: Oct
- FR: Oct

**Event 2: Day**  `DRAFT, FACT`
- EN: 02
- FR: 02

**Event 2: Type**  `DRAFT, FACT`
- EN: Four-week series
- FR: Série de quatre semaines

**Event 2: Time**  `DRAFT, FACT`
- EN: Thursdays, 19:00
- FR: Les jeudis, 19 h

**Event 2: Title**  `DRAFT, FACT`
- EN: Nervous System Basics
- FR: Système nerveux : les bases

**Event 2: Description**  `DRAFT, FACT`
- EN: Four evenings on how stress physiology works and what genuinely shifts it — breath, rhythm, food, sleep, touch.
- FR: Quatre soirées sur la physiologie du stress et ce qui la transforme réellement : souffle, rythme, alimentation, sommeil, toucher.

**Event 2: Price**  `DRAFT, FACT`
- EN: $220
- FR: 220 $

**Event 2: Places**  `DRAFT, FACT`
- EN: 10 places
- FR: 10 places

**Event 3: Month**  `DRAFT, FACT`
- EN: Oct
- FR: Oct

**Event 3: Day**  `DRAFT, FACT`
- EN: 25
- FR: 25

**Event 3: Type**  `DRAFT, FACT`
- EN: Workshop
- FR: Atelier

**Event 3: Time**  `DRAFT, FACT`
- EN: 10:00 – 13:00
- FR: 10 h – 13 h

**Event 3: Title**  `DRAFT, FACT`
- EN: Ayurvedic Autumn Kitchen
- FR: Cuisine ayurvédique d’automne

**Event 3: Description**  `DRAFT, FACT`
- EN: Cooking for the shift into cold season: spice combinations, digestion, and three simple weekday meals. We eat together at the end.
- FR: Cuisiner pour l’entrée dans la saison froide : combinaisons d’épices, digestion et trois repas simples de semaine. Nous mangeons ensemble à la fin.

**Event 3: Price**  `DRAFT, FACT`
- EN: $85
- FR: 85 $

**Event 3: Places**  `DRAFT, FACT`
- EN: 12 places
- FR: 12 places

**Event 4: Month**  `DRAFT, FACT`
- EN: Nov
- FR: Nov

**Event 4: Day**  `DRAFT, FACT`
- EN: 14
- FR: 14

**Event 4: Type**  `DRAFT, FACT`
- EN: Group session
- FR: Séance de groupe

**Event 4: Time**  `DRAFT, FACT`
- EN: 19:00 – 20:15
- FR: 19 h – 20 h 15

**Event 4: Title**  `DRAFT, FACT`
- EN: Guided Deep Rest
- FR: Repos profond guidé

**Event 4: Description**  `DRAFT, FACT`
- EN: A group craniosacral and breathwork session. Bring a blanket; leave loose. Monthly through winter.
- FR: Une séance de groupe en craniosacral et respiration. Apportez une couverture ; repartez détendu. Chaque mois pendant l’hiver.

**Event 4: Price**  `DRAFT, FACT`
- EN: $35
- FR: 35 $

**Event 4: Places**  `DRAFT, FACT`
- EN: 16 places
- FR: 16 places

**Event 5: Month**  `DRAFT, FACT`
- EN: Dec
- FR: Déc

**Event 5: Day**  `DRAFT, FACT`
- EN: 05
- FR: 05

**Event 5: Type**  `DRAFT, FACT`
- EN: Talk
- FR: Causerie

**Event 5: Time**  `DRAFT, FACT`
- EN: 18:00 – 19:30
- FR: 18 h – 19 h 30

**Event 5: Title**  `DRAFT, FACT`
- EN: Sleep, Honestly
- FR: Le sommeil, honnêtement

**Event 5: Description**  `DRAFT, FACT`
- EN: What fifteen years of practice has taught me about why people cannot sleep, and the handful of things that reliably help.
- FR: Ce que quinze ans de pratique m’ont appris sur les raisons de l’insomnie, et le petit nombre de choses qui aident vraiment.

**Event 5: Price**  `DRAFT, FACT`
- EN: Free
- FR: Gratuit

**Event 5: Places**  `DRAFT, FACT`
- EN: RSVP required
- FR: RSVP requis

**Private groups: title**  `DRAFT`
- EN: Private and corporate groups
- FR: Groupes privés et entreprises

**Private groups: text**  `DRAFT`
- EN: Workshops can be adapted for teams, studios and private groups, in the clinic or at your space. Tell me the group and the time you have.
- FR: Les ateliers peuvent être adaptés aux équipes, aux studios et aux groupes privés, en clinique ou chez vous. Dites-moi la taille du groupe et le temps disponible.

**Private groups: button**  `DRAFT`
- EN: Inquire about a private group
- FR: Informations pour un groupe privé

> ⚠ Event 5 says "what fifteen years of practice has taught me": same years issue.

## 6. Digital Library

> ⚠ Product titles, page counts and prices are placeholders until the client clarifies what she sells.

**Label**  `DRAFT`
- EN: Digital Library
- FR: Bibliothèque numérique

**H1**  `DRAFT`
- EN: Guides you can start using tonight.
- FR: Des guides que vous pouvez utiliser dès ce soir.

**Lead**  `DRAFT`
- EN: Everything I would tell you in a consultation, written down and organised. Purchase, download immediately, keep it forever.
- FR: Tout ce que je vous dirais en consultation, écrit et organisé. Achetez, téléchargez immédiatement, gardez-le pour toujours.

**Badge 1**  `DRAFT`
- EN: Instant download
- FR: Téléchargement immédiat

**Badge 2**  `DRAFT`
- EN: PDF and EPUB
- FR: PDF et EPUB

**Badge 3**  `DRAFT`
- EN: Free lifetime updates
- FR: Mises à jour à vie

**Buy button**  `DRAFT`
- EN: Buy Now
- FR: Acheter

**How it works (3 steps)**  `NEW / FR-NEW`
- EN: Purchase → instant download link → lifetime access
- FR: Achat → lien de téléchargement immédiat → accès à vie

**Product 1: Format**  `PLACEHOLDER`
- EN: E-book · 84 pages
- FR: Livre numérique · 84 pages

**Product 1: Title**  `PLACEHOLDER`
- EN: The Winter Protocol
- FR: Le protocole d’hiver

**Product 1: Description**  `PLACEHOLDER`
- EN: A full Ayurvedic guide to the Montréal cold season: food, oils, routine and the herbs that hold you through February.
- FR: Un guide ayurvédique complet pour la saison froide montréalaise : alimentation, huiles, routine et les plantes qui vous portent jusqu’en février.

**Product 1: Price**  `PLACEHOLDER`
- EN: $24
- FR: 24 $

**Product 2: Format**  `PLACEHOLDER`
- EN: Guide · 42 pages
- FR: Guide · 42 pages

**Product 2: Title**  `PLACEHOLDER`
- EN: Sleep, Rebuilt
- FR: Reconstruire le sommeil

**Product 2: Description**  `PLACEHOLDER`
- EN: The staged plan I give clients who have not slept properly in years. Evening rhythm, herbs, and what to stop doing.
- FR: Le plan progressif que je remets aux clients qui ne dorment plus vraiment depuis des années. Rythme du soir, plantes, et ce qu’il faut cesser.

**Product 2: Price**  `PLACEHOLDER`
- EN: $18
- FR: 18 $

**Product 3: Format**  `PLACEHOLDER`
- EN: E-book · 96 pages
- FR: Livre numérique · 96 pages

**Product 3: Title**  `PLACEHOLDER`
- EN: Digestion First
- FR: La digestion d’abord

**Product 3: Description**  `PLACEHOLDER`
- EN: Why most complaints begin in the gut, and a twelve-week path back to steady digestion without elimination diets.
- FR: Pourquoi la plupart des troubles commencent dans l’intestin, et un parcours de douze semaines vers une digestion stable, sans régime d’exclusion.

**Product 3: Price**  `PLACEHOLDER`
- EN: $26
- FR: 26 $

**Product 4: Format**  `PLACEHOLDER`
- EN: Guide · 36 pages
- FR: Guide · 36 pages

**Product 4: Title**  `PLACEHOLDER`
- EN: Self-Massage at Home
- FR: L’auto-massage à la maison

**Product 4: Description**  `PLACEHOLDER`
- EN: Abhyanga, jaw and neck release, and a ten-minute daily sequence. Illustrated, step by step.
- FR: Abhyanga, relâchement de la mâchoire et de la nuque, et une séquence quotidienne de dix minutes. Illustré, étape par étape.

**Product 4: Price**  `PLACEHOLDER`
- EN: $16
- FR: 16 $

**Product 5: Format**  `PLACEHOLDER`
- EN: Workbook · 58 pages
- FR: Cahier · 58 pages

**Product 5: Title**  `PLACEHOLDER`
- EN: The Nervous System Reset
- FR: Réinitialiser le système nerveux

**Product 5: Description**  `PLACEHOLDER`
- EN: Six weeks of daily practices for burnout recovery, with tracking pages and weekly reflections.
- FR: Six semaines de pratiques quotidiennes pour sortir de l’épuisement, avec pages de suivi et réflexions hebdomadaires.

**Product 5: Price**  `PLACEHOLDER`
- EN: $22
- FR: 22 $

**Product 6: Format**  `PLACEHOLDER`
- EN: Bundle · 4 titles
- FR: Ensemble · 4 titres

**Product 6: Title**  `PLACEHOLDER`
- EN: The Complete Library
- FR: La bibliothèque complète

**Product 6: Description**  `PLACEHOLDER`
- EN: All four guides plus the workbook, and every future edition, at a single price.
- FR: Les quatre guides et le cahier, ainsi que toutes les éditions futures, à un seul prix.

**Product 6: Price**  `PLACEHOLDER`
- EN: $68
- FR: 68 $

## 7. Shop (hidden from the menu)

**Label**  `DRAFT`
- EN: Shop
- FR: Boutique

**H1**  `DRAFT`
- EN: The clinic shelf, available to order.
- FR: La tablette de la clinique, offerte en ligne.

**Lead**  `DRAFT`
- EN: Herbs, oils and tools I use in practice, plus digital bundles. Shipped within Canada or picked up at the clinic.
- FR: Les plantes, les huiles et les outils que j’utilise en pratique, ainsi que des ensembles numériques. Livraison au Canada ou cueillette à la clinique.

**Buy button**  `DRAFT`
- EN: Buy Now
- FR: Acheter

**Add to cart button**  `NEW / FR-NEW`
- EN: Add to Cart
- FR: Ajouter au panier

**Product 1: Category**  `PLACEHOLDER`
- EN: Herbal
- FR: Plantes

**Product 1: Name**  `PLACEHOLDER`
- EN: Calm Evening Tea
- FR: Tisane du soir

**Product 1: Description**  `PLACEHOLDER`
- EN: Chamomile, tulsi, rose and licorice. 100 g loose leaf, small batch.
- FR: Camomille, tulsi, rose et réglisse. 100 g en feuilles, petite production.

**Product 1: Price**  `PLACEHOLDER`
- EN: $22
- FR: 22 $

**Product 2: Category**  `PLACEHOLDER`
- EN: Ayurvedic
- FR: Ayurveda

**Product 2: Name**  `PLACEHOLDER`
- EN: Warming Abhyanga Oil
- FR: Huile d’Abhyanga réchauffante

**Product 2: Description**  `PLACEHOLDER`
- EN: Sesame base infused with ashwagandha and ginger. For vata seasons. 200 ml.
- FR: Base de sésame infusée d’ashwagandha et de gingembre. Pour les saisons vata. 200 ml.

**Product 2: Price**  `PLACEHOLDER`
- EN: $34
- FR: 34 $

**Product 3: Category**  `PLACEHOLDER`
- EN: Ayurvedic
- FR: Ayurveda

**Product 3: Name**  `PLACEHOLDER`
- EN: Cooling Coconut Oil
- FR: Huile de coco rafraîchissante

**Product 3: Description**  `PLACEHOLDER`
- EN: Coconut with brahmi and sandalwood, for heat and irritation. 200 ml.
- FR: Coco, brahmi et santal, pour la chaleur et les irritations. 200 ml.

**Product 3: Price**  `PLACEHOLDER`
- EN: $32
- FR: 32 $

**Product 4: Category**  `PLACEHOLDER`
- EN: Tools
- FR: Accessoires

**Product 4: Name**  `PLACEHOLDER`
- EN: Copper Tongue Scraper
- FR: Gratte-langue en cuivre

**Product 4: Description**  `PLACEHOLDER`
- EN: The two-second morning practice I recommend to everyone.
- FR: La pratique matinale de deux secondes que je recommande à tout le monde.

**Product 4: Price**  `PLACEHOLDER`
- EN: $14
- FR: 14 $

**Product 5: Category**  `PLACEHOLDER`
- EN: Digital
- FR: Numérique

**Product 5: Name**  `PLACEHOLDER`
- EN: Winter Protocol Bundle
- FR: Ensemble Protocole d’hiver

**Product 5: Description**  `PLACEHOLDER`
- EN: The Winter Protocol e-book with the warming oil and digestive tea.
- FR: Le livre Protocole d’hiver avec l’huile réchauffante et la tisane digestive.

**Product 5: Price**  `PLACEHOLDER`
- EN: $72
- FR: 72 $

**Product 6: Category**  `PLACEHOLDER`
- EN: Gift
- FR: Cadeau

**Product 6: Name**  `PLACEHOLDER`
- EN: Session Gift Card
- FR: Carte-cadeau séance

**Product 6: Description**  `PLACEHOLDER`
- EN: A 75-minute treatment of their choosing, valid for one year.
- FR: Un traitement de 75 minutes au choix, valable un an.

**Product 6: Price**  `PLACEHOLDER`
- EN: $130
- FR: 130 $

## 8. Blog (native Wix Blog inside the page frame)

**Page label**  `NEW / FR-NEW`
- EN: Journal
- FR: Journal

**H1**  `NEW / FR-NEW`
- EN: Notes on rest, recovery and everyday wellbeing.
- FR: Notes sur le repos, la récupération et le bien-être au quotidien.

Posts: the native Blog block fills the main area. The 2 existing posts stay (French). Their text lives in Wix and is not part of this file.

## 9. Native Wix block states (visual reference only)

These are inside Wix apps (Stores, checkout, Events). The design shows a labeled placeholder; the final wording is set in each Wix app.

**Checkout: Total**  `PLACEHOLDER`
- EN: Total
- FR: Total

**Checkout: Card number**  `PLACEHOLDER`
- EN: Card number
- FR: Numéro de carte

**Checkout: Pay**  `PLACEHOLDER`
- EN: Pay
- FR: Payer

**Checkout: Processing**  `PLACEHOLDER`
- EN: Processing payment…
- FR: Traitement du paiement…

**Checkout: Done: title**  `PLACEHOLDER`
- EN: Payment complete
- FR: Paiement complété

**Checkout: Done: text**  `PLACEHOLDER`
- EN: Your download is ready and a copy has been sent to your email.
- FR: Votre téléchargement est prêt et une copie a été envoyée par courriel.

**Checkout: Close**  `PLACEHOLDER`
- EN: Close
- FR: Fermer

**Checkout: secure note**  `NEW / FR-NEW`
- EN: Secure checkout
- FR: Paiement sécurisé

> ⚠ The mockup says "This is a demo transaction". Removed. Real checkout wording comes from Wix.

## 10. SEO drafts per page (title ≤ 60, description ≤ 155)

`NEW` / `FR-NEW`. First pass only. The full SEO rewrite (keywords, headings, schema, alt text) is a separate step.

**Home**
- EN title (57): Massage & Naturopathy in Montréal | Aspring Health Center
- EN description (142): Massage therapy, naturopathy, craniosacral therapy and Ayurvedic care with Victoria in Plateau-Mont-Royal, Montréal. Book your session online.
- FR title (58): Massage et naturopathie à Montréal | Aspring Health Center
- FR description (145): Massothérapie, naturopathie, thérapie crânio-sacrée et soins ayurvédiques avec Victoria, sur le Plateau-Mont-Royal à Montréal. Réservez en ligne.

**Massage Therapy**
- EN title (51): Massage Therapy in Montréal | Aspring Health Center
- EN description (144): Functional health, deep tissue, anti-cortisol and facial massage in Plateau-Mont-Royal. See sessions and prices, then book online with Victoria.
- FR title (48): Massothérapie à Montréal | Aspring Health Center
- FR description (146): Massage fonctionnel, tissus profonds, anti-cortisol et facial sur le Plateau-Mont-Royal. Découvrez séances et tarifs, puis réservez avec Victoria.

**Naturopathy & Ayurveda**
- EN title (58): Naturopathy & Ayurveda in Montréal | Aspring Health Center
- EN description (130): Root-cause naturopathy, Ayurvedic consultations, craniosacral therapy and Shirodhara in Montréal. Personalized care with Victoria.
- FR title (59): Naturopathie et Ayurveda à Montréal | Aspring Health Center
- FR description (145): Naturopathie axée sur les causes, consultations ayurvédiques, thérapie crânio-sacrée et Shirodhara à Montréal. Soins personnalisés avec Victoria.

**Retreats**
- EN title (51): Wellness Retreats in Québec | Aspring Health Center
- EN description (139): Small-group wellness retreats in Québec led by Victoria: bodywork, Ayurvedic meals and deep rest. See upcoming dates and ask about a place.
- FR title (53): Retraites bien-être au Québec | Aspring Health Center
- FR description (141): Retraites bien-être en petit groupe au Québec avec Victoria : soins du corps, repas ayurvédiques et repos profond. Dates et demande de place.

**Events**
- EN title (54): Workshops & Events in Montréal | Aspring Health Center
- EN description (123): Evening workshops, group sessions and talks on Ayurveda, nervous-system care and sleep in Montréal. See dates and register.
- FR title (57): Ateliers et événements à Montréal | Aspring Health Center
- FR description (133): Ateliers du soir, séances de groupe et conférences sur l'ayurvéda, le système nerveux et le sommeil à Montréal. Dates et inscription.

**Digital Library**
- EN title (57): Digital Wellness Guides & E-books | Aspring Health Center
- EN description (113): Practical Ayurvedic and wellness guides by Victoria on sleep, digestion, self-massage and more. Instant download.
- FR title (51): Guides bien-être numériques | Aspring Health Center
- FR description (125): Guides pratiques d'ayurvéda et de bien-être par Victoria : sommeil, digestion, auto-massage et plus. Téléchargement immédiat.

**Shop**: `noindex` (hidden page).

## Not carried over (conflicts with real data)

The mockup's massage types (Therapeutic Swedish, Deep Tissue, Craniosacral, Ayurvedic Abhyanga, Prenatal) and price table ($110–$155), invented testimonials, and "Tue – Sat" hours. The full original is in `content/source/mockup-copy.json` and `client-brief/`.