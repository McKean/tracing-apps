# COVID-19 Contact-Tracing Apps Tracker

Tracing apps are proliferating; this repo is trying to keep track of them, with an eye on privacy implications.

## Contact-Tracing App Projects

* #### [CoEpi](https://www.coepi.org) | Community Epidemiology In Action

	**Status**: In development

	**Technical synopsis**

	The CoEpi app uses Bluetooth to record an anonymized list of close-proximity Interactions with other users.

	* In an Interaction, apps exchange temporary Contact-Event-Numbers (CEN). The other user's CEN is stored along with a timestamp for when the interaction occurred. Temporary CENs are deterministically generated from a cryptographic Key, which is private by default.
	* User can choose to upload their Key, along with symptoms, to a public database
	* The app downloads Keys and their associated Symptoms from the public database and searches local Interactions records to determine if any of the User's interactions were with symptomatic users
	* No location data is captured

* #### [TraceTogether](https://www.tracetogether.gov.sg/) (Singapore)

	> By using time-varying tokens, the app does keep
	the users private from each other. A user has no
	way of knowing who the tokens stored in their app
	belong to, except by linking them to the time the
	token was received. However, the app provides
	little to no privacy for infected individuals; after
	an infected individual is compelled to release their
	data, the Singaporean government can build a list
	of all the other people they have been in contact
	with.
	(https://arxiv.org/abs/2003.11511)

	Open source version announced 2020/03/25:
	https://www.cnbc.com/2020/03/25/coronavirus-singapore-to-make-contact-tracing-tech-open-source.html

* #### [Private Kit: Safe Paths](http://safepaths.mit.edu/)

	**Status**: Apps are live, backends and agency integrations in development

	**Technical synopsis**

	The Safe Paths app saves the user's GPS location data to a local encrypted store.

	* When a user tests positive, they can choose to give their location records to a health professional, who then manually redacts personally-identifiable information and publishes the redacted data to a public database.
	* The app downloads location data of infected cases from the public database to search against locally-stored location history

* #### [covidnearyou.org](https://covidnearyou.org/)

	**Status**: Live, ~2000 reported symptoms/test-results

	Self-reported symptoms/test-results aggregated by zipcode

**Need more info:**

* [enigmampc/SafeTrace](https://github.com/enigmampc/SafeTrace)
* [corona-trace](https://corona-trace.github.io/)
* https://stopcorona.me/
* [crowdcovid.com](https://crowdcovid.com/): [github.com/olieidel/corona-tracker](https://github.com/olieidel/corona-tracker)
* ...and lots more — you can help track the tracers by making a PR for one that's missing, or adding info to any of the above.

## Research, Analysis, and Design proposals

* [Anonymous Retrospective Broadcasts](https://gist.github.com/hdevalence/fefba3153b30e60537e84f7d2551b295) ([Henry de Valence](https://github.com/hdevalenc))
* [Contact Tracing Mobile Apps for COVID-19: Privacy Considerations and Related Trade-offs](https://arxiv.org/abs/2003.11511) (Hyunghoon Cho, Daphne Ippolito, Yun William Yu)

## Related trackers and resources

* [Privacy International: Tracking the Global Response to COVID-19](https://privacyinternational.org/examples/tracking-global-response-covid-19)
* [Electronic Frontier Foundation: COVID-19 and Digital Rights](https://www.eff.org/issues/covid-19)
* [Top10VPN COVID-19 Digital Rights Tracker](https://www.top10vpn.com/news/surveillance/covid-19-digital-rights-tracker/)
* https://www.digitalvaccine.net/

## Are you developing a Tracing App?

Please PR an overview of your system into this repo!

## Meta

We're pondering the clearest way to present the above information, and how to aggregate and present community concerns and discussion about the individual projects.

## I want to contribute to covid-apps-tracker

Great! It's easy:

1. Agree with our [Code of Conduct](./CODE_OF_CONDUCT.md)
2. Post an Issue or PR to this repository
