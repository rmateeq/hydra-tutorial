## Components of an AI-driven App

Let's begin with a simplified view of an app at an abstract level. Irrespective of whether it is a mobile, web, or desktop app, it usually consists of the user interface at the top, followed by the domain-specific logic layer, and storage at the bottom. This basic view is shown in the figure below.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/209483960-65dd2d7c-4c6f-4012-9f76-171826529009.png" width="520" height="255" />
</p>

So where does AI fit in? It primarily exists in parallel to the logic layer incorporating intelligence. As with the logic layer, AI also interacts with both UI layer (to supply the intelligent outcomes in the context of a user) and the storage layer (to keep the required data and intelligent models). The figure below presents this simple schematic view of an AI-driven app where the AI modules exist alongside the logic layer, complemented by the external data pipes (in addition to intra-app communication) to interact with the external sources/events, if and when necessary.

<p align="center">
<img src="https://user-images.githubusercontent.com/7511849/209484060-a6e629f3-fdaa-42ec-ae57-8ab84a9af6ff.png" width="520" height="255" />
</p>

Having visualized the addition of a parallel component of AI at the logic layer, let's delve into answering why are this tutorial and platform there (i.e., how building AI is different from developing traditional software). Why cannot AI be added to an existing software architecture just like any other update?
