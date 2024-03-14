# 💻 07. webserver
## devcontainers
Het beheren en implementeren van webprojecten is geëvolueerd met de opkomst van moderne ontwikkelingspraktijken. Versiebeheer en DevContainers zijn nu essentiële instrumenten voor het effectief beheren en implementeren van websites. In dit hoofdstuk zullen we deze benaderingen verkennen en begrijpen hoe ze de traditionele FTP/SSH-methoden kunnen vervangen.
### Versiebeheer
Versiebeheersystemen zijn cruciaal voor het bijhouden van wijzigingen in de broncode van een project. Git is veelgebruikt en wordt vaak gekozen vanwege zijn flexibiliteit en kracht. Hier zijn enkele kernconcepten van Git:
#### Branching en Merging
Git maakt het mogelijk om parallelle ontwikkelingslijnen te creëren, bekend als "branches". Dit stelt ontwikkelaars in staat om afzonderlijke functies of wijzigingen te implementeren zonder de hoofdcode te beïnvloeden. Het samenvoegen van branches (merging) zorgt voor het integreren van deze wijzigingen.
#### Commit en Historie
Elke wijziging in Git wordt vastgelegd in een "commit". Dit helpt bij het bijhouden van de historie van wijzigingen, waardoor ontwikkelaars gemakkelijk door verschillende versies kunnen navigeren en eerdere wijzigingen kunnen begrijpen.
#### Remote Repositories
Met Git kunnen ontwikkelaars samenwerken via externe repositories. Platforms zoals GitHub, GitLab en Bitbucket bieden ruimte voor het delen van code en het beheren van projecten op afstand.
### devcontainers
DevContainers, ofwel ontwikkelingscontainers, bieden een geïsoleerde en reproduceerbare omgeving voor het ontwikkelen van applicaties. Deze containers bevatten alle benodigde software, dependencies en configuraties die nodig zijn voor een project. Visual Studio Code (VSCode) biedt ondersteuning voor DevContainers, waardoor ontwikkelaars gemakkelijk een uniforme ontwikkelingsomgeving kunnen instellen.
#### voordelen van DevContainers
- **Consistente Ontwikkelingsomgeving**: Elke ontwikkelaar werkt met dezelfde geconfigureerde container, waardoor inconsistente ontwikkelingsomgevingen worden geminimaliseerd.
- **Eenvoudige Onboarding**: Nieuwe teamleden kunnen snel aan de slag gaan door simpelweg de DevContainer-configuratie te gebruiken.
- **Reproduceerbaarheid**: DevContainers garanderen dat een applicatie in dezelfde omstandigheden kan worden uitgevoerd, ongeacht waar deze wordt geïmplementeerd.
### deployment met versiebeheer en DevContainers
Nu we de basisbeginselen hebben begrepen, laten we kijken hoe versiebeheer en DevContainers samenwerken voor effectieve implementatie:
1. **Codebeheer met Git**:
- Start een Git-repository voor je project.
- Gebruik branches om nieuwe functies of bugfixes te ontwikkelen.
- Voer regelmatig commits uit om wijzigingen vast te leggen.
2. **DevContainers Configuratie**:
- Voeg een DevContainer-configuratiebestand toe (.devcontainer/devcontainer.json) aan je Git-repository.
- Definieer de benodigde software, extensies en instellingen voor de container.
3. **Continuous Integration (CI) en Continuous Deployment (CD)**:
- Gebruik CI/CD-tools zoals GitHub Actions, GitLab CI, of Azure Pipelines om automatische tests en implementaties te configureren.
- De CI/CD-pijplijn kan de DevContainer gebruiken om een consistente omgeving te garanderen tijdens tests en implementatie.
4. **Implementatie met Containers**:
- Containers, zoals Docker, kunnen worden gebruikt om applicaties te isoleren en eenvoudig te implementeren.
- De DevContainer-configuratie kan worden aangepast voor productieomgevingen met minimale aanpassingen.

Door Git en DevContainers te combineren, kun je een gestroomlijnd ontwikkelingsproces en een consistente implementatieomgeving creëren. Dit maakt de overgang van ontwikkeling naar implementatie soepeler en betrouwbaarder dan traditionele FTP/SSH-methoden.

## 📚 bronnen
- [AP cursus webtechnologie > serverbeheer](https://apwt.gitbook.io/webtechnologie/serverbeheer/intro)