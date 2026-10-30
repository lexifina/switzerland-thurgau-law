# Thurgau: law history in git

The law of the canton of Thurgau (Kanton Thurgau, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `ch-tg/`. The federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, the canton's official language, exactly as the canton publishes it.

## What this repository holds

314 acts with 913 versions so far: the cantonal constitution, the cantonal laws (Gesetze) in force and 228 Verordnungen and Reglemente in force, in the order of the systematic collection, added in parts. Other decrees and decisions, intercantonal agreements and repealed acts are not included yet.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `101-kv/` | Verfassung des Kantons Thurgau (RB 101) | 4 | oldest version available, then each consolidated version: 1 January 2012 to 15 June 2026 |
| `131-1-gemg/` | Gesetz über die Gemeinden (RB 131.1) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 June 2022 |
| `141-1-kbug/` | Gesetz über das Kantons- und Gemeindebürgerrecht (RB 141.1) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2018 |
| `142-15-erg/` | Gesetz über das Einwohnerregister sowie kantonale Register (RB 142.15) | 2 | as enacted, then each consolidated version: 1 August 2009 to 1 August 2013 |
| `161-1-stwg/` | Gesetz über das Stimm- und Wahlrecht (RB 161.1) | 2 | oldest version available, then each consolidated version: 1 September 2011 to 1 August 2014 |
| `162/` | Gesetz über die Ausübung des Petitionsrechtes (RB 162) | 1 | as enacted, 1 January 1990 |
| `170-1-vrg/` | Gesetz über die Verwaltungsrechtspflege (RB 170.1) | 7 | oldest version available, then each consolidated version: 1 January 2011 to 1 June 2024 |
| `170-3-verantwortlichkeitsgesetz/` | Gesetz über die Verantwortlichkeit (RB 170.3) | 3 | oldest version available, then each consolidated version: 1 June 2004 to 1 October 2025 |
| `170-5/` | Gesetz über die öffentlichen Bekanntmachungen (RB 170.5) | 1 | one version (the oldest available), 1 January 1991 |
| `170-6-offentlichkeitsgesetz-offg/` | Gesetz über das Öffentlichkeitsprinzip (RB 170.6) | 1 | as enacted, 1 June 2022 |
| `170-7-tg-dsg/` | Gesetz über den Datenschutz (RB 170.7) | 3 | oldest version available, then each consolidated version: 1 July 2012 to 1 June 2022 |
| `170-8-statg/` | Gesetz über die öffentliche Statistik (RB 170.8) | 1 | as enacted, 1 January 2022 |
| `176-1-anwg/` | Anwaltsgesetz (RB 176.1) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2022 |
| `186-1/` | Gesetz über kirchliche Paritätsverhältnisse und Verträge (RB 186.1) | 1 | as enacted, 1 July 2000 |
| `188-22-lkg/` | Gesetz der Katholischen Synode über die Katholische Landeskirche des Kantons Thurgau (RB 188.22) | 2 | as enacted, then each consolidated version: 14 March 1970 to 1 January 2022 |
| `188-23-kgg/` | Gesetz der Katholischen Synode über die katholischen Kirchgemeinden des Kantons Thurgau (RB 188.23) | 3 | as enacted, then each consolidated version: 1 March 1997 to 1 January 2026 |
| `188-25-fagkl/` | Finanzausgleichsgesetz der Katholischen Landeskirche Thurgau (RB 188.25) | 1 | one version (the oldest available), 1 January 2024 |
| `210-1-eg-zgb/` | Einführungsgesetz zum Schweizerischen Zivilgesetzbuch (RB 210.1) | 13 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2028 |
| `211-415-tg-bewg/` | Gesetz über den Erwerb von Grundstücken durch Personen im Ausland (RB 211.415) | 1 | one version (the oldest available), 19 November 1997 |
| `211-441-tg-geoig/` | Gesetz über Geoinformation (RB 211.441) | 1 | as enacted, 1 January 2012 |
| `271-1-zsrg/` | Gesetz über die Zivil- und Strafrechtspflege (RB 271.1) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 October 2025 |
| `311-1-eg-stgb/` | Einführungsgesetz zum Schweizerischen Strafrecht (RB 311.1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2022 |
| `411-11-vg/` | Gesetz über die Volksschule (RB 411.11) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2024 |
| `411-61-beitragsgesetz/` | Gesetz über Beitragsleistungen an die Schulgemeinden (RB 411.61) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2020 |
| `413-11-gbm/` | Gesetz über die Berufsbildung und die Mittelschulen (Sekundarstufe II) (RB 413.11) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2018 |
| `414-2-tertiarbildungsgesetz/` | Gesetz über die tertiäre Bildung (RB 414.2) | 2 | oldest version available, then each consolidated version: 1 January 2009 to 1 May 2015 |
| `415-1-sportforderungsgesetz/` | Gesetz über die Förderung von Sport und Bewegung (RB 415.1) | 1 | as enacted, 1 June 2012 |
| `416-1-stipendiengesetz-stipg/` | Gesetz über Ausbildungsbeiträge (RB 416.1) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 August 2013 |
| `432-10-archivg/` | Gesetz über Aktenführung und Archivierung (RB 432.10) | 2 | as enacted, then each consolidated version: 1 January 2021 to 1 June 2022 |
| `442-1-kulturg/` | Gesetz über die Kulturförderung und die Kulturpflege (RB 442.1) | 2 | as enacted, then each consolidated version: 1 January 1994 to 1 January 2017 |
| `450-1-tg-nhg/` | Gesetz zum Schutz und zur Pflege der Natur und der Heimat (RB 450.1) | 3 | oldest version available, then each consolidated version: 1 January 2008 to 1 July 2023 |
| `520-1-eg-bzg/` | Einführungsgesetz zur Bundesgesetzgebung über den Zivilschutz (RB 520.1) | 1 | one version (the oldest available), 1 September 2005 |
| `530-1/` | Gesetz über die Bewältigung von ausserordentlichen Lagen (RB 530.1) | 1 | as enacted, 1 September 2005 |
| `551-1-polg/` | Polizeigesetz (RB 551.1) | 3 | as enacted, then each consolidated version: 1 July 2012 to 1 June 2024 |
| `554-11-log/` | Gesetz über die Ladenöffnungszeiten (RB 554.11) | 1 | one version (the oldest available), 1 January 2009 |
| `554-51-gastg/` | Gastgewerbe- und Alkoholhandelsgesetz (RB 554.51) | 2 | oldest version available, then each consolidated version: 1 January 2003 to 1 January 2024 |
| `611-1-fhg/` | Finanzhaushaltsgesetz (RB 611.1) | 2 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2024 |
| `613-1-fag/` | Gesetz über den Finanzausgleich der Politischen Gemeinden (RB 613.1) | 2 | oldest version available, then each consolidated version: 1 January 2014 to 1 January 2019 |
| `632-1-ggg/` | Gesetz über die Gebühren und Gemengsteuern der Grundbuchämter und Notariate (RB 632.1) | 2 | oldest version available, then each consolidated version: 1 January 2003 to 1 January 2016 |
| `640-1-stg/` | Steuergesetz (RB 640.1) | 12 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2029 |
| `641-2-hundeg/` | Hundegesetz (RB 641.2) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 May 2025 |
| `641-8-eschg/` | Gesetz über die Erbschafts- und Schenkungssteuer (RB 641.8) | 1 | one version (the oldest available), 1 January 2013 |
| `690/` | Gesetz über das Salzregal (RB 690) | 1 | as enacted, 1 October 1975 |
| `700-pbg/` | Planungs- und Baugesetz (RB 700) | 6 | as enacted, then each consolidated version: 1 January 2013 to 1 June 2024 |
| `708-1-feuerschutzgesetz-fsg/` | Gesetz über den Feuerschutz (RB 708.1) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2021 |
| `710-tg-entg/` | Gesetz über die Enteignung (RB 710) | 1 | one version (the oldest available), 1 June 2004 |
| `720-1-gob/` | Gesetz über das öffentliche Beschaffungswesen (RB 720.1) | 1 | as enacted, 1 April 2022 |
| `721-1-wbsng/` | Gesetz über den Wasserbau und den Schutz vor gravitativen Naturgefahren (RB 721.1) | 3 | oldest version available, then each consolidated version: 1 January 2008 to 1 March 2019 |
| `721-3/` | Gesetz über die öffentliche Zugänglichkeit der Ufer (RB 721.3) | 1 | one version (the oldest available), 1 January 1993 |
| `721-8-wng/` | Wassernutzungsgesetz (RB 721.8) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 June 2024 |
| `723-1-ung/` | Gesetz über die Nutzung des Untergrundes (RB 723.1) | 2 | as enacted, then each consolidated version: 1 April 2016 to 1 January 2021 |
| `725-1-strwg/` | Gesetz über Strassen und Wege (RB 725.1) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 July 2023 |
| `731-1-eng/` | Gesetz über die Energienutzung (RB 731.1) | 5 | oldest version available, then each consolidated version: 1 January 2013 to 19 June 2023 |
| `734-1/` | Einführungsgesetz zum Bundesgesetz über die Stromversorgung (RB 734.1) | 2 | as enacted, then each consolidated version: 1 July 2010 to 1 June 2024 |
| `741-1-svag/` | Gesetz über die Strassenverkehrsabgaben (RB 741.1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 July 2023 |
| `742-1-fovg/` | Gesetz über die Förderung des öffentlichen Verkehrs (RB 742.1) | 2 | oldest version available, then each consolidated version: 1 January 2002 to 1 January 2016 |
| `747-2/` | Gesetz über die Wasserfahrzeugsteuer (RB 747.2) | 1 | one version (the oldest available), 1 January 2000 |
| `810-1-gg/` | Gesundheitsgesetz (RB 810.1) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `812-4-gta/` | Gesetz über Plakatwerbung und Jugendschutz für Tabak und Alkohol (RB 812.4) | 2 | as enacted, then each consolidated version: 1 January 2007 to 1 January 2023 |
| `812-7-gsbm/` | Gesetz über den Solidaritätsbeitrag für Betroffene von Medikamententests (RB 812.7) | 1 | as enacted, 1 January 2025 |
| `814-04-abfallgesetz/` | Gesetz über die Abfallbewirtschaftung (RB 814.04) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `814-20-eg-gschg/` | Einführungsgesetz zum Bundesgesetz über den Schutz der Gewässer (RB 814.20) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 June 2024 |
| `819-1-vetg/` | Gesetz über das Veterinärwesen (RB 819.1) | 1 | as enacted, 1 April 2022 |
| `822-9-rtg/` | Ruhetagsgesetz (RB 822.9) | 2 | oldest version available, then each consolidated version: 1 January 2003 to 1 January 2026 |
| `831-1-eg-ahvg-ivg/` | Einführungsgesetz zu den Bundesgesetzen über die Alters- und Hinterlassenenversicherung und über die Invalidenversicherung (RB 831.1) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2014 |
| `831-2-eg-ahvg-ivg/` | Einführungsgesetz zu den Bundesgesetzen über die Alters- und Hinterlassenenversicherung und über die Invalidenversicherung (RB 831.2) | 1 | as enacted, 1 May 2026 |
| `831-3/` | Gesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (RB 831.3) | 1 | as enacted, 1 January 2008 |
| `832-1-tg-kvg/` | Krankenversicherungsgesetz (RB 832.1) | 7 | oldest version available, then each consolidated version: 1 January 2012 to 1 February 2026 |
| `836-1-familienzulagengesetz-tg-famzg/` | Gesetz über die Familienzulagen (RB 836.1) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2021 |
| `836-4-alig/` | Gesetz über die Inkassohilfe für familienrechtliche Unterhaltsbeiträge und die Bevorschussung von Kinderalimenten (RB 836.4) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2022 |
| `837-1-masg/` | Gesetz über Massnahmen gegen die Arbeitslosigkeit und zur Standortförderung (RB 837.1) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 April 2026 |
| `842-1/` | Gesetz über Massnahmen zur Förderung des Wohnungsbaues (RB 842.1) | 1 | one version (the oldest available), 1 January 1973 |
| `850-1-shg/` | Sozialhilfegesetz (RB 850.1) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2027 |
| `850-2-flembg/` | Gesetz über die Finanzierung von Leistungen für erwachsene Menschen mit Behinderung (RB 850.2) | 1 | as enacted, 1 January 2025 |
| `861-1/` | Gesetz über die familienergänzende Kinderbetreuung (RB 861.1) | 1 | as enacted, 1 January 2005 |
| `910-1/` | Landwirtschaftsgesetz (RB 910.1) | 2 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2016 |
| `913-1/` | Gesetz über Flur und Garten (RB 913.1) | 2 | oldest version available, then each consolidated version: 1 May 2001 to 1 June 2015 |
| `913-2-meliorationsgesetz-melg/` | Gesetz über Bodenverbesserungen und landwirtschaftliche Hochbauten (RB 913.2) | 2 | oldest version available, then each consolidated version: 1 April 2002 to 1 January 2013 |
| `921-1-waldg/` | Waldgesetz (RB 921.1) | 3 | oldest version available, then each consolidated version: 1 April 2012 to 1 January 2026 |
| `922-1-jg/` | Gesetz über die Jagd und den Schutz wildlebender Säugetiere und Vögel (RB 922.1) | 4 | as enacted, then each consolidated version: 1 January 1993 to 1 April 2023 |
| `923-1-fig/` | Fischereigesetz (RB 923.1) | 2 | oldest version available, then each consolidated version: 1 April 2002 to 1 January 2023 |
| `935-1-lsg/` | Gesetz über den Lotterie- und Sportfonds (RB 935.1) | 1 | as enacted, 1 January 2021 |
| `935-2-ksg/` | Kleinspielgesetz (RB 935.2) | 1 | as enacted, 1 January 2021 |
| `951-1-tkb-g/` | Gesetz über die Thurgauer Kantonalbank (RB 951.1) | 2 | oldest version available, then each consolidated version: 1 October 2011 to 1 October 2013 |
| `954-1-ekt-g/` | Gesetz über das Elektrizitätswerk des Kantons Thurgau (RB 954.1) | 1 | as enacted, 1 January 2001 |
| `956-1-gebaudeversicherungsgesetz-gebg/` | Gesetz über die Gebäudeversicherung (RB 956.1) | 2 | oldest version available, then each consolidated version: 1 January 2003 to 1 January 2021 |
| `112-11-hzv/` | Verordnung des Regierungsrates über die Hoheitszeichen (RB 112.11) | 1 | as enacted, 1 June 2019 |
| `131-21/` | Verordnung über das Rechnungswesen der Gemeinden (RB 131.21) | 2 | as enacted, then each consolidated version: 1 June 2013 to 1 May 2023 |
| `141-11-kbuv/` | Verordnung des Regierungsrates zum Gesetz über das Kantons- und Gemeindebürgerrecht (RB 141.11) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2018 |
| `142-151-erv/` | Einwohnerregisterverordnung (RB 142.151) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2024 |
| `142-211/` | Verordnung des Regierungsrates zum Ausländer- und Integrationsgesetz, zum Freizügigkeitsabkommen und zum Asylgesetz (RB 142.211) | 5 | as enacted, then each consolidated version: 1 October 2009 to 1 January 2022 |
| `143-2/` | Verordnung des Regierungsrates über den Vollzug der Bundesgesetzgebung über die Ausweise für Schweizer Staatsangehörige (RB 143.2) | 2 | oldest version available, then each consolidated version: 1 March 2012 to 1 January 2020 |
| `161-11-stwv/` | Verordnung über das Stimm- und Wahlrecht (RB 161.11) | 3 | oldest version available, then each consolidated version: 1 September 2011 to 1 August 2025 |
| `170-15-ubermittlungsverordnung-veu/` | Verordnung des Regierungsrates betreffend die elektronische Übermittlung im Rahmen von Verwaltungs-, Zivil-, Straf- sowie Schuldbetreibungs- und Konkursverfahren (RB 170.15) | 2 | as enacted, then each consolidated version: 1 July 2015 to 28 March 2026 |
| `170-21-tg-vlv/` | Verordnung des Regierungsrates über das Vernehmlassungsverfahren (RB 170.21) | 1 | as enacted, 1 April 2017 |
| `170-51/` | Verordnung des Regierungsrates über Abgabe und Bezug des Thurgauer Rechtsbuches und des Amtsblattes des Kantons Thurgau (RB 170.51) | 1 | as enacted, 1 January 1992 |
| `170-71-datenschutzverordnung-tg-dsv/` | Verordnung des Regierungsrates über den Datenschutz (RB 170.71) | 2 | as enacted, then each consolidated version: 5 December 2008 to 1 March 2013 |
| `171-12/` | Reglement des Grossen Rates über das Begnadigungsverfahren (RB 171.12) | 1 | as enacted, 28 May 2008 |
| `172-1-grr/` | Geschäftsreglement des Regierungsrates (RB 172.1) | 6 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2023 |
| `172-31-itv/` | Informatikverordnung (RB 172.31) | 5 | oldest version available, then each consolidated version: 1 January 2010 to 1 January 2025 |
| `172-33/` | Reglement des Regierungsrates für das Personalamt (RB 172.33) | 1 | one version (the oldest available), 1 June 2004 |
| `173-12/` | Verordnung über die personelle Organisation der Bezirksgerichte (RB 173.12) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2024 |
| `173-21-vvog/` | Verordnung des Verwaltungsgerichts über die Organisation und den Geschäftsgang (RB 173.21) | 2 | as enacted, then each consolidated version: 1 January 2013 to 4 May 2024 |
| `173-31/` | Verordnung des Verwaltungsgerichts über die Organisation und den Geschäftsgang der Rekurskommission (RB 173.31) | 1 | as enacted, 1 January 2013 |
| `176-11-anwv/` | Anwaltsverordnung (RB 176.11) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `176-61/` | Verordnung des Verwaltungsgerichtes über den Anwaltstarif für Streitigkeiten vor dem Verwaltungsgericht, dem Versicherungsgericht, der Enteignungskommission und den Rekurskommissionen (RB 176.61) | 1 | as enacted, 1 October 2009 |
| `177-22-besoldungsverordnung-besvo/` | Verordnung des Grossen Rates über die Besoldung des Staatspersonals (RB 177.22) | 7 | oldest version available, then each consolidated version: 30 June 2012 to 1 October 2025 |
| `177-41-pensionskassenverordnung-pkvo/` | Verordnung des Grossen Rates über die berufliche Vorsorge des Staatspersonals und der Lehrpersonen (RB 177.41) | 3 | as enacted, then each consolidated version: 1 January 2006 to 1 January 2020 |
| `177-42-pkr/` | Pensionskassenreglement (RB 177.42) | 14 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `177-112-rsv/` | Rechtsstellungsverordnung (RB 177.112) | 10 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `177-223-rrv-besvo/` | Verordnung des Regierungsrates zur Besoldungsverordnung (RB 177.223) | 16 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `177-250-lbv/` | Verordnung des Grossen Rates über die Besoldung der Lehrpersonen (RB 177.250) | 3 | oldest version available, then each consolidated version: 1 January 2006 to 1 January 2024 |
| `186-11/` | Verordnung des Regierungsrates zum Gesetz über kirchliche Paritätsverhältnisse und Verträge (RB 186.11) | 1 | as enacted, 1 October 2005 |
| `187-13-rechtspflegeverordnung/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Rechtspflege der Thurgauischen Landeskirche (RB 187.13) | 4 | oldest version available, then each consolidated version: 1 June 2004 to 1 January 2023 |
| `187-14/` | Geschäftsreglement der Evangelischen Synode des Kantons Thurgau (RB 187.14) | 3 | oldest version available, then each consolidated version: 1 September 2006 to 1 August 2025 |
| `187-22/` | Besoldungsverordnung der Evangelischen Synode des Kantons Thurgau (RB 187.22) | 6 | oldest version available, then each consolidated version: 1 January 2006 to 1 January 2026 |
| `187-23/` | Verordnung der Evangelischen Synode des Kantons Thurgau zur Rechtsstellung der ordinierten Amtspersonen (RB 187.23) | 3 | oldest version available, then each consolidated version: 1 January 2020 to 1 January 2026 |
| `187-24/` | Verordnung des Evangelischen Kirchenrates des Kantons Thurgau zur Gottesdienstleitung durch Laien (RB 187.24) | 2 | as enacted, then each consolidated version: 1 April 2002 to 1 June 2016 |
| `187-25/` | Verordnung über die Amtsübergabe bei Pfarrwechseln (RB 187.25) | 2 | as enacted, then each consolidated version: 1 January 1980 to 1 May 2019 |
| `187-27/` | Verordnung der Evangelischen Synode des Kantons Thurgau betreffend die berufliche Vorsorge für die Arbeitnehmerinnen und Arbeitnehmer der Evangelischen Kirchgemeinden und der Evangelischen Landeskirche (RB 187.27) | 3 | as enacted, then each consolidated version: 1 January 1995 to 1 January 2020 |
| `187-28/` | Verordnung des Evangelischen Kirchenrates des Kantons Thurgau über die Bestätigungswahl der ordinierten Amtsträger und Amtsträgerinnen (RB 187.28) | 1 | as enacted, 1 June 2004 |
| `187-29-stipendienreglement/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Ausrichtung von kirchlichen Ausbildungsbeiträgen (RB 187.29) | 2 | as enacted, then each consolidated version: 1 January 1992 to 1 September 2015 |
| `187-122/` | Verordnung der Evangelischen Synode des Kantons Thurgau «Kirche, Kind und Jugend» (RB 187.122) | 2 | oldest version available, then each consolidated version: 1 August 2013 to 1 August 2025 |
| `187-124/` | Verordnung der Evangelischen Synode des Kantons Thurgau über Visitationen (RB 187.124) | 2 | as enacted, then each consolidated version: 1 January 1973 to 1 August 2014 |
| `187-131/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Organisation der Aufsichtskommission der Kirchgemeinde (RB 187.131) | 1 | as enacted, 1 June 2004 |
| `187-132/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Aufgaben und die Tätigkeit der Ombudsstelle (RB 187.132) | 2 | as enacted, then each consolidated version: 1 August 2014 to 1 June 2021 |
| `187-141/` | Geschäftsreglement des Evangelischen Kirchenrates des Kantons Thurgau (RB 187.141) | 2 | as enacted, then each consolidated version: 1 June 2008 to 1 January 2023 |
| `187-143-entschadigungsverordnung/` | Verordnung der Synode über Entschädigungen in der Evangelischen Landeskirche des Kantons Thurgau (RB 187.143) | 6 | as enacted, then each consolidated version: 1 January 2013 to 1 January 2024 |
| `187-144/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Abgeltung von kirchlichen Diensten zwischen Kirchgemeinden (RB 187.144) | 2 | as enacted, then each consolidated version: 1 April 2002 to 1 August 2016 |
| `187-151/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Einteilung der Dekanatskreise und die Organisation der Kapitel (RB 187.151) | 2 | as enacted, then each consolidated version: 1 January 2004 to 1 April 2018 |
| `187-153/` | Verordnung des Evangelischen Kirchenrates des Kantons Thurgau zum kirchlichen Stimm- und Wahlrecht (RB 187.153) | 4 | as enacted, then each consolidated version: 20 August 2003 to 15 September 2025 |
| `187-171-finanzausgleichsverordnung/` | Verordnung der Evangelischen Synode des Kantons Thurgau über Leistungen der Landeskirche zu Gunsten von finanzschwachen Kirchgemeinden (RB 187.171) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `187-172/` | Verordnung des Kirchenrates zur Verordnung der Evangelischen Synode des Kantons Thurgau über Leistungen der Landeskirche zu Gunsten von finanzschwachen Kirchgemeinden (RB 187.172) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2022 |
| `187-181/` | Reglement der Evangelischen Synode des Kantons Thurgau über den Fonds zur Mitfinanzierung von Aufgaben der Diakonie, der kirchlichen Jugendarbeit und des Gemeindebaus (RB 187.181) | 2 | as enacted, then each consolidated version: 1 January 2013 to 1 January 2023 |
| `187-182/` | Reglement des Evangelischen Kirchenrates über den Fonds für Mütter in Not (RB 187.182) | 1 | as enacted, 1 July 2005 |
| `187-183/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Unterstützung von Institutionen (RB 187.183) | 1 | as enacted, 1 January 2006 |
| `187-191/` | Verordnung des Evangelischen Kirchenrates des Kantons Thurgau über die Verwaltung und das Rechnungswesen (RB 187.191) | 3 | as enacted, then each consolidated version: 1 January 2018 to 1 January 2025 |
| `187-222/` | Verordnung des Evangelischen Kirchenrates des Kantons Thurgau betreffend die Weiterbildung und Studienurlaube (RB 187.222) | 1 | as enacted, 1 January 2011 |
| `187-225/` | Verordnung der Evangelischen Synode des Kantons Thurgau über die Pfarramtsstellvertretung (RB 187.225) | 1 | as enacted, 1 July 2003 |
| `187-231/` | Verordnung der Evangelischen Synode des Kantons Thurgau über Ökumene, Mission, Diakonie und Entwicklungszusammenarbeit (RB 187.231) | 1 | as enacted, 1 August 2009 |
| `187-261/` | Verordnung des Evangelischen Kirchenrates des Kantons Thurgau über die Aktenführung und Archivierung (RB 187.261) | 1 | as enacted, 1 January 2019 |
| `188-26/` | Verordnung der Katholischen Synode des Kantons Thurgau über die Pensionskasse der Katholischen Landeskirche (PKL) (RB 188.26) | 1 | as enacted, 1 July 2013 |
| `188-27/` | Stipendienreglement der Katholischen Landeskirche (RB 188.27) | 1 | as enacted, 1 January 2010 |
| `188-28/` | Verordnung der Katholischen Synode über den Religionsunterricht an der Volksschule (RB 188.28) | 2 | as enacted, then each consolidated version: 1 August 2001 to 1 August 2016 |
| `188-211-besoldungsverordnung/` | Verordnung der Katholischen Synode betreffend die Besoldungen, Taggelder und Entschädigungen (RB 188.211) | 5 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2026 |
| `188-212/` | Verordnung der Katholischen Synode betreffend Kloster Fischingen (RB 188.212) | 1 | as enacted, 1 January 2011 |
| `188-215/` | Verordnung der Katholischen Synode über die Gemeindeseelsorge und die caritative Diakonie (RB 188.215) | 1 | as enacted, 17 August 1996 |
| `188-216/` | Verordnung der Katholischen Synode des Kantons Thurgau über die Anderssprachigenseelsorge (RB 188.216) | 1 | as enacted, 1 January 2013 |
| `188-217/` | Reglement des Katholischen Kirchenrates betreffend Bau- und Strukturhilfefonds (RB 188.217) | 1 | as enacted, 27 April 1991 |
| `188-241-grkk/` | Geschäftsreglement des Katholischen Kirchenrats des Kantons Thurgau (RB 188.241) | 1 | as enacted, 1 July 2026 |
| `188-251-rwv/` | Verordnung des Katholischen Kirchenrats über das Rechnungswesen (RB 188.251) | 2 | as enacted, then each consolidated version: 1 January 2005 to 1 January 2026 |
| `188-252-avfa/` | Ausführungsverordnung des Katholischen Kirchenrats zum Finanzausgleichsgesetz der Katholischen Landeskirche Thurgau (RB 188.252) | 2 | as enacted, then each consolidated version: 1 January 2013 to 1 July 2024 |
| `188-272/` | Verordnung des Katholischen Kirchenrates des Kantons Thurgau betreffend die Stiftungsaufsicht (RB 188.272) | 1 | as enacted, 29 January 1983 |
| `188-291-av/` | Archivverordnung des Katholischen Kirchenrats (RB 188.291) | 2 | as enacted, then each consolidated version: 2 March 1996 to 1 January 2024 |
| `211-34-inventarverordnung/` | Verordnung des Obergerichts über die Errichtung des öffentlichen Inventars (RB 211.34) | 1 | as enacted, 1 January 2011 |
| `211-111/` | Verordnung des Regierungsrates über das Zivilstandswesen (RB 211.111) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2020 |
| `211-412/` | Verordnung des Regierungsrates zum Bundesgesetz über das bäuerliche Bodenrecht (RB 211.412) | 1 | as enacted, 1 January 1994 |
| `211-423/` | Verordnung des Regierungsrates betreffend die Organisation der Verschreibungsämter und Aufsichtsbehörden über die Viehverpfändung (RB 211.423) | 1 | one version (the oldest available), 1 January 2011 |
| `211-431-gnv/` | Verordnung über das Grundbuch- und Notariatswesen (RB 211.431) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `211-439-vgnp/` | Verordnung über die Grundbuch- und Notariatsprüfung (RB 211.439) | 3 | oldest version available, then each consolidated version: 6 November 2004 to 1 January 2025 |
| `211-442-tg-geoiv/` | Geoinformationsverordnung (RB 211.442) | 6 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `211-443-vv/` | Vermessungsverordnung (RB 211.443) | 3 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `221-42/` | Verordnung des Regierungsrates über das Handelsregister (RB 221.42) | 1 | as enacted, 1 June 1992 |
| `221-214/` | Verordnung des Regierungsrates zur Bundesgesetzgebung über den Konsumkredit (RB 221.214) | 1 | as enacted, 1 March 2006 |
| `221-226/` | Verordnung des Regierungsrates zum Bundesgesetz über die landwirtschaftliche Pacht (LPG) vom 4. Oktober 1985 (RB 221.226) | 1 | one version (the oldest available), 1 January 2011 |
| `221-251/` | Verordnung des Regierungsrates zum Bundesgesetz vom 28. September 1956 über die Allgemeinverbindlich-erklärung von Gesamtarbeitsverträgen (RB 221.251) | 1 | as enacted, 23 December 1978 |
| `221-252/` | Verordnung des Regierungsrates über den Normalarbeitsvertrag für hauswirtschaftliche Arbeitsverhältnisse im Kanton Thurgau (RB 221.252) | 1 | one version (the oldest available), 28 August 2010 |
| `221-253/` | Verordnung des Regierungsrates über den Normalarbeitsvertrag für landwirtschaftliche Arbeitsverhältnisse im Kanton Thurgau (RB 221.253) | 1 | as enacted, 1 April 2006 |
| `221-254-nav-24h/` | Verordnung des Regierungsrates über den Normalarbeitsvertrag für Angestellte im Haushaltsdienst mit 24-Stunden-Betreuung (RB 221.254) | 1 | as enacted, 28 November 2020 |
| `271-31-informationsverordnung/` | Verordnung des Obergerichts über die Information in Zivil- und Strafgerichtsverfahren und die Akteneinsicht durch Dritte (RB 271.31) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 April 2023 |
| `281-12-voabk/` | Verordnung über die Organisation des Amtes für Betreibungs- und Konkurswesen (RB 281.12) | 2 | as enacted, then each consolidated version: 1 June 2016 to 1 January 2022 |
| `311-41/` | Verordnung des Regierungsrates betreffend den Vollzug der Interkantonalen Vereinbarung über die computergestützte Zusammenarbeit der Kantone bei der Aufklärung von Gewaltdelikten vom 2. April 2009 (ViCLAS-Konkordat) (RB 311.41) | 1 | as enacted, 1 January 2011 |
| `311-61-ovsta/` | Verordnung des Regierungsrates über die Organisation der Staatsanwaltschaft (RB 311.61) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2021 |
| `313-11/` | Verordnung betreffend die Zuständigkeiten der kantonalen Behörden gemäss Bundesgesetz über das Verwaltungsstrafrecht (VStrR) (RB 313.11) | 1 | as enacted, 1 January 2011 |
| `331-11/` | Verordnung des Regierungsrates über das Strafregister (RB 331.11) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2016 |
| `340-31-jvv/` | Justizvollzugsverordnung (RB 340.31) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 December 2021 |
| `410-31/` | Verordnung des Regierungsrates über die Vereinigung von Schulgemeinden und Politischen Gemeinden (RB 410.31) | 1 | one version (the oldest available), 1 January 2013 |
| `411-111-vsv/` | Volksschulverordnung (RB 411.111) | 9 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2024 |
| `411-114-rsv-vs/` | Verordnung über die Rechtsstellung der Lehrpersonen an den Volksschulen (RB 411.114) | 13 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2025 |
| `411-115-beurteilungsreglement/` | Reglement über die Beurteilung in der Volksschule (RB 411.115) | 3 | as enacted, then each consolidated version: 1 August 2008 to 1 August 2021 |
| `411-116/` | Verordnung des Regierungsrates über die Rechtsstellung der sonderpädagogischen Fachpersonen an der Volksschule (RB 411.116) | 2 | as enacted, then each consolidated version: 1 January 2010 to 1 January 2015 |
| `411-411-sonderschulv/` | Verordnung des Regierungsrates über die Sonderschulung, Heilpädagogische Früherziehung, Spitalschulung und spezielle Unterstützungsangebote (RB 411.411) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2021 |
| `411-611-beitragsverordnung/` | Verordnung zum Gesetz über Beitragsleistungen an die Schulgemeinden (RB 411.611) | 13 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `411-661-msv/` | Musikschulverordnung (RB 411.661) | 6 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2024 |
| `412-211-bbo/` | Verordnung über die Organisation des Berufsbildungswesens (RB 412.211) | 7 | oldest version available, then each consolidated version: 11 September 2010 to 1 January 2025 |
| `412-212-bbg/` | Verordnung über die berufliche Grundbildung (RB 412.212) | 8 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `412-213-bbw/` | Verordnung des Regierungsrates über die höhere Berufsbildung und die berufsorientierte Weiterbildung (RB 412.213) | 2 | as enacted, then each consolidated version: 1 January 2015 to 1 August 2016 |
| `412-214-bbb/` | Verordnung über die Brückenangebote, die niederschwelligen Ausbildungsangebote und die kantonalen Integrationskurse (RB 412.214) | 5 | as enacted, then each consolidated version: 1 January 2015 to 1 January 2026 |
| `412-215-bbm/` | Verordnung über die Berufsmaturität an den Berufsfachschulen (RB 412.215) | 4 | as enacted, then each consolidated version: 1 August 2015 to 1 August 2026 |
| `412-225-reglement-hf-betriebswirtschaft/` | Reglement des Departements für Erziehung und Kultur über die Ausbildung zur diplomierten Betriebswirtschafterin HF oder zum diplomierten Betriebswirtschafter HF (RB 412.225) | 3 | as enacted, then each consolidated version: 29 January 2011 to 1 October 2022 |
| `412-227/` | Reglement des Departements für Erziehung und Kultur über die Ausbildung zur diplomierten Pflegefachperson HF (RB 412.227) | 5 | oldest version available, then each consolidated version: 1 August 2012 to 1 January 2026 |
| `412-228-reglement-hf-technik/` | Reglement des Departements für Erziehung und Kultur über die Bildungsgänge der höheren Fachschule am Bildungszentrum für Technik (RB 412.228) | 1 | as enacted, 1 August 2025 |
| `413-141-rsv-bm/` | Verordnung über die Rechtsstellung der Lehrpersonen an den Berufsfach- und Mittelschulen (RB 413.141) | 11 | oldest version available, then each consolidated version: 1 August 2011 to 1 January 2024 |
| `413-142/` | Verordnung über die Organisation der Mittelschulen (RB 413.142) | 2 | as enacted, then each consolidated version: 1 January 2008 to 1 April 2022 |
| `413-223/` | Verordnung über die Aufnahme in die Maturitäts- und Fachmittelschulen (RB 413.223) | 3 | oldest version available, then each consolidated version: 1 August 2005 to 1 February 2023 |
| `413-224/` | Verordnung über die Ausbildung an der Pädagogischen Maturitätsschule Kreuzlingen (RB 413.224) | 5 | oldest version available, then each consolidated version: 1 August 2012 to 1 August 2028 |
| `413-226-mkv/` | Verordnung über die Maturitätsabteilung an den thurgauischen Kantonsschulen (RB 413.226) | 5 | oldest version available, then each consolidated version: 1 August 2008 to 1 August 2028 |
| `413-228-ims-verordnung/` | Verordnung über die Informatikmittelschule der Kantonsschule Frauenfeld (RB 413.228) | 4 | oldest version available, then each consolidated version: 1 January 2008 to 1 August 2026 |
| `413-253-rrv-fms/` | Verordnung über die Ausbildung an den Fachmittelschulen der thurgauischen Kantonsschulen (RB 413.253) | 10 | oldest version available, then each consolidated version: 1 January 2011 to 1 August 2025 |
| `413-282/` | Reglement über die Maturitätsprüfungen an der Thurgauisch-Schaffhauserischen Maturitätsschule für Erwachsene (RB 413.282) | 2 | oldest version available, then each consolidated version: 1 February 2008 to 1 February 2024 |
| `413-284/` | Personalreglement der Thurgauisch-Schaffhauserischen Maturitätsschule für Erwachsene (RB 413.284) | 4 | as enacted, then each consolidated version: 1 February 2014 to 1 February 2024 |
| `414-21/` | Reglement über die Studiengänge Primarstufe Schuljahre 1 bis 5 und Primarstufe Schuljahre 3 bis 8 der Pädagogischen Hochschule Thurgau (RB 414.21) | 5 | as enacted, then each consolidated version: 14 November 2009 to 1 September 2023 |
| `414-22/` | Reglement über den Masterstudiengang Frühe Kindheit der Pädagogischen Hochschule Thurgau und der Universität Konstanz (RB 414.22) | 2 | as enacted, then each consolidated version: 8 October 2011 to 29 June 2013 |
| `414-24/` | Gebührenreglement der Pädagogischen Hochschule Thurgau (RB 414.24) | 4 | oldest version available, then each consolidated version: 6 October 2012 to 18 September 2023 |
| `414-25/` | Reglement über den Studiengang Sekundarstufe II der Pädagogischen Hochschule Thurgau (RB 414.25) | 4 | oldest version available, then each consolidated version: 13 November 2010 to 11 May 2024 |
| `414-26/` | Reglement über den Studiengang Sekundarstufe I der Pädagogischen Hochschule Thurgau (RB 414.26) | 4 | as enacted, then each consolidated version: 19 March 2011 to 18 September 2023 |
| `414-27/` | Personalreglement der Pädagogischen Hochschule Thurgau (RB 414.27) | 7 | as enacted, then each consolidated version: 8 May 2010 to 14 June 2025 |
| `414-28/` | Geschäftsreglement der Pädagogischen Hochschule Thurgau (RB 414.28) | 4 | as enacted, then each consolidated version: 25 September 2004 to 14 June 2025 |
| `416-11-stipv/` | Stipendienverordnung (RB 416.11) | 7 | oldest version available, then each consolidated version: 1 August 2010 to 1 August 2025 |
| `416-21-schulgeldverordnung/` | Verordnung des Regierungsrates betreffend die Übernahme von Schulgeldern (RB 416.21) | 1 | one version (the oldest available), 1 August 2004 |
| `432-101/` | Gebührenreglement Staatsarchiv (RB 432.101) | 1 | as enacted, 1 May 2026 |
| `432-211/` | Verordnung des Regierungsrates über die Bibliotheken (RB 432.211) | 1 | one version (the oldest available), 24 September 2005 |
| `432-311-museumsverordnung/` | Verordnung über die kantonalen Museen (RB 432.311) | 2 | as enacted, then each consolidated version: 1 January 1999 to 1 January 2015 |
| `442-11-kulturv/` | Verordnung des Regierungsrates zum Gesetz über die Kulturförderung und die Kulturpflege (RB 442.11) | 3 | oldest version available, then each consolidated version: 24 December 2005 to 1 May 2018 |
| `450-11-tg-nhv/` | Verordnung zum Schutz und zur Pflege der Natur und der Heimat (RB 450.11) | 6 | oldest version available, then each consolidated version: 1 November 2012 to 1 July 2023 |
| `511-54/` | Verordnung des Regierungsrates über die Zuständigkeit für Disziplinarstrafen und den Vollzug von Urteilen im Bereich des Militärstrafgesetzes (RB 511.54) | 1 | as enacted, 1 January 2013 |
| `514-52/` | Verordnung des Regierungsrates über den Vollzug der eidgenössischen Waffengesetzgebung (RB 514.52) | 1 | one version (the oldest available), 1 July 2012 |
| `520-11/` | Verordnung des Regierungsrates zum Einführungsgesetz zur Bundesgesetzgebung über den Zivilschutz (RB 520.11) | 3 | as enacted, then each consolidated version: 1 January 2005 to 1 February 2015 |
| `530-11/` | Verordnung des Regierungsrates zum Gesetz über die Bewältigung von ausserordentlichen Lagen (RB 530.11) | 2 | as enacted, then each consolidated version: 1 September 2005 to 1 January 2022 |
| `541-11/` | Verordnung des Regierungsrates über den Vollzug des Konkordates über Massnahmen gegen Gewalt anlässlich von Sportveranstaltungen und des Bundesgesetzes über Massnahmen zur Wahrung der inneren Sicherheit (RB 541.11) | 2 | as enacted, then each consolidated version: 1 January 2010 to 1 February 2015 |
| `551-6/` | Verordnung des Regierungsrates über die Datenbearbeitung durch die Kantonspolizei (RB 551.6) | 1 | as enacted, 1 July 2012 |
| `551-11-polv/` | Polizeiverordnung (RB 551.11) | 4 | as enacted, then each consolidated version: 1 July 2012 to 1 June 2024 |
| `551-41-beforderungsverordnung-befv/` | Verordnung über die Beförderungen der Polizistinnen und Polizisten (RB 551.41) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 October 2025 |
| `552-12/` | Verordnung des Regierungsrates zur Interkantonalen Vereinbarung über die polizeiliche Zusammenarbeit vom 21. Januar 1976 (RB 552.12) | 1 | one version (the oldest available), 1 January 1991 |
| `553-1/` | Verordnung des Regierungsrates über die privaten polizeiähnlichen Tätigkeiten (RB 553.1) | 1 | one version (the oldest available), 1 January 1991 |
| `554-121/` | Verordnung des Regierungsrates über den Vollzug der eidgenössischen Reisendengewerbegesetzgebung (RB 554.121) | 1 | as enacted, 1 January 2003 |
| `611-11-fhv/` | Finanzhaushaltsverordnung (RB 611.11) | 7 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `611-14/` | Verordnung des Regierungsrates über den Vollzug des Bundesbeschlusses über die Sperrung und die Freigabe von Krediten im Voranschlag der Schweizerischen Eidgenossenschaft (Kreditsperrungsbeschluss, KSB) (RB 611.14) | 1 | as enacted, 1 January 1997 |
| `611-21/` | Verordnung über die Überprüfung der Lohngleichheitsanalyse (RB 611.21) | 1 | as enacted, 1 January 2022 |
| `613-11-fav/` | Finanzausgleichsverordnung (RB 613.11) | 5 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2019 |
| `631-1-vgv/` | Verordnung des Grossen Rates über die Gebühren der kantonalen Verwaltungsbehörden (RB 631.1) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2016 |
| `631-11-rrv-vgv/` | Verordnung des Regierungsrates über die Gebühren der kantonalen Verwaltungsbehörden (RB 631.11) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2016 |
| `638-1-vgg/` | Verordnung des Grossen Rates über die Gebühren der Strafverfolgungs- und Gerichtsbehörden (RB 638.1) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2022 |
| `640-11-stv/` | Steuerverordnung (RB 640.11) | 12 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2025 |
| `640-12-schav/` | Grundstückschätzungsverordnung (RB 640.12) | 4 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2024 |
| `640-13-vakp/` | Verordnung über den Ausgleich der kalten Progression (RB 640.13) | 3 | as enacted, then each consolidated version: 1 January 2023 to 1 January 2025 |
| `640-14-ev/` | Verordnung über die Entschädigung der Gemeindesteuerämter (RB 640.14) | 1 | as enacted, 1 January 2025 |
| `640-21/` | Berufskostenverordnung (RB 640.21) | 4 | oldest version available, then each consolidated version: 1 January 2009 to 1 January 2022 |
| `640-22/` | Verordnung über die Anrechnung ausländischer Quellensteuern (RB 640.22) | 2 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2020 |
| `641-21-hundev/` | Hundeverordnung (RB 641.21) | 4 | oldest version available, then each consolidated version: 1 January 2008 to 1 May 2025 |
| `642-2/` | Verordnung des Regierungsrates zum Bundesgesetz über die Verrechnungssteuer (VStG) (RB 642.2) | 1 | one version (the oldest available), 1 January 2001 |
| `642-11/` | Verordnung des Regierungsrates zum Bundesgesetz über die direkte Bundessteuer (DBG) (RB 642.11) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2016 |
| `661-11/` | Verordnung des Regierungsrates zum Bundesgesetz über die Wehrpflichtersatzabgabe (RB 661.11) | 2 | oldest version available, then each consolidated version: 12 January 2008 to 8 February 2014 |
| `700-1-pbv/` | Verordnung zum Planungs- und Baugesetz und zur Interkantonalen Vereinbarung über die Harmonisierung der Baubegriffe (RB 700.1) | 11 | as enacted, then each consolidated version: 1 January 2013 to 6 July 2024 |
| `700-3-ksv/` | Kleinsiedlungsverordnung (RB 700.3) | 2 | as enacted, then each consolidated version: 16 May 2020 to 8 October 2022 |
| `700-41-gvksv/` | Verordnung zum Gesetz über Vereinbarungen zur Milderung finanzieller Härtefälle von raumplanerischen Massnahmen in Kleinsiedlungen (RB 700.41) | 1 | as enacted, 1 April 2023 |
| `708-11-feuerschutzverordnung-fsv/` | Verordnung des Regierungsrates zum Gesetz über den Feuerschutz (RB 708.11) | 4 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2021 |
| `720-11-vob/` | Verordnung über das öffentliche Beschaffungswesen (RB 720.11) | 1 | as enacted, 1 April 2022 |
| `721-11-wbsnv/` | Verordnung des Regierungsrates zum Gesetz über den Wasserbau und den Schutz vor gravitativen Naturgefahren (RB 721.11) | 5 | oldest version available, then each consolidated version: 1 January 2008 to 30 May 2020 |
| `721-81-wnv/` | Verordnung des Regierungsrates zum Wassernutzungsgesetz (RB 721.81) | 2 | oldest version available, then each consolidated version: 14 April 2012 to 1 January 2016 |
| `723-11-unv/` | Verordnung des Regierungsrates zum Gesetz über die Nutzung des Untergrundes (RB 723.11) | 1 | as enacted, 1 April 2016 |
| `725-10-strwv/` | Verordnung zum Gesetz über Strassen und Wege (RB 725.10) | 3 | oldest version available, then each consolidated version: 1 January 2008 to 1 July 2023 |
| `725-11/` | Verordnung des Regierungsrates zur Einführung des Bundesgesetzes über die Nationalstrassen (RB 725.11) | 2 | as enacted, then each consolidated version: 18 November 1997 to 1 June 2015 |
| `725-12-ggv/` | Verordnung des Regierungsrates über die Gebühren für den gesteigerten Gemeingebrauch von Kantonsstrassen und -wegen (RB 725.12) | 1 | as enacted, 1 January 2018 |
| `725-16/` | Verordnung des Regierungsrates über die Offenhaltung der Versorgungsrouten für Ausnahmetransporte (RB 725.16) | 3 | as enacted, then each consolidated version: 18 November 1997 to 1 March 2019 |
| `731-11-env/` | Energienutzungsverordnung (RB 731.11) | 4 | oldest version available, then each consolidated version: 29 October 2011 to 1 January 2025 |
| `741-2/` | Verordnung des Regierungsrates zum Strassenverkehrsgesetz und den Nebenerlassen (RB 741.2) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2018 |
| `741-11-svav/` | Strassenverkehrsabgabenverordnung (RB 741.11) | 3 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2023 |
| `742-11-fovv/` | Verordnung des Regierungsrates zum Gesetz über die Förderung des öffentlichen Verkehrs (RB 742.11) | 2 | oldest version available, then each consolidated version: 29 October 2011 to 1 January 2016 |
| `746-1-rlv/` | Verordnung zur eidgenössischen Rohrleitungsgesetzgebung (RB 746.1) | 2 | as enacted, then each consolidated version: 1 April 2011 to 2 April 2022 |
| `747-11/` | Verordnung des Regierungsrates über die Gebühren der Schiffahrtskontrolle (RB 747.11) | 1 | as enacted, 1 January 1998 |
| `747-21/` | Verordnung des Regierungsrates zum Gesetz über die Wasserfahrzeugsteuer (RB 747.21) | 1 | as enacted, 1 January 2000 |
| `748-11/` | Verordnung des Regierungsrates zur Luftfahrtgesetzgebung des Bundes (RB 748.11) | 1 | one version (the oldest available), 1 January 2011 |
| `811-121-gesbv/` | Gesundheitsberufeverordnung (RB 811.121) | 7 | oldest version available, then each consolidated version: 1 October 2009 to 1 July 2024 |
| `811-314/` | Verordnung des Regierungsrates über die Rechtsstellung der Patienten und Patientinnen (RB 811.314) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 September 2015 |
| `812-2-hmv/` | Heilmittelverordnung (RB 812.2) | 5 | as enacted, then each consolidated version: 1 January 2002 to 1 July 2024 |
| `812-41-vta/` | Verordnung über Plakatwerbung und Jugendschutz für Tabak und Alkohol (RB 812.41) | 1 | as enacted, 1 January 2023 |
| `812-51/` | Verordnung des Regierungsrates zum Vollzug der eidgenössischen Gesetzgebung zum Schutz vor Passivrauchen (RB 812.51) | 1 | as enacted, 1 May 2010 |
| `814-03-usgv/` | Verordnung zur Umweltschutzgesetzgebung (RB 814.03) | 3 | as enacted, then each consolidated version: 31 December 2011 to 1 July 2023 |
| `814-011/` | Verordnung zur Umweltverträglichkeitsprüfung (RB 814.011) | 5 | oldest version available, then each consolidated version: 19 September 2009 to 23 December 2023 |
| `814-041-abfallverordnung/` | Verordnung zum Gesetz über die Abfallbewirtschaftung (RB 814.041) | 2 | oldest version available, then each consolidated version: 31 December 2011 to 1 January 2025 |
| `814-211-rrv-eg-gschg/` | Verordnung zum Bundesgesetz und zum Einführungsgesetz zum Bundesgesetz über den Schutz der Gewässer (RB 814.211) | 3 | oldest version available, then each consolidated version: 1 April 1999 to 29 March 2025 |
| `814-811-rrv-chemg/` | Verordnung des Regierungsrates zur Chemikaliengesetzgebung des Bundes (RB 814.811) | 1 | one version (the oldest available), 31 December 2011 |
| `817-21/` | Verordnung des Regierungsrates über den Vollzug der Bundesgesetzgebung über Lebensmittel und Gebrauchsgegenstände (RB 817.21) | 2 | oldest version available, then each consolidated version: 1 June 2004 to 1 April 2018 |
| `818-12/` | Verordnung des Regierungsrates über den Vollzug des Bundesgesetzes über die Bekämpfung übertragbarer Krankheiten des Menschen (RB 818.12) | 2 | oldest version available, then each consolidated version: 1 January 2000 to 1 May 2016 |
| `819-11-vetv/` | Verordnung über das Veterinärwesen (RB 819.11) | 3 | as enacted, then each consolidated version: 1 April 2022 to 1 May 2025 |
| `821-421/` | Verordnung des Regierungsrates betreffend Bestellung einer kantonalen Einigungsstelle (RB 821.421) | 1 | one version (the oldest available), 18 November 1997 |
| `822-11/` | Verordnung des Regierungsrates zur Bundesgesetzgebung über die Arbeit in Industrie, Gewerbe und Handel (RB 822.11) | 1 | one version (the oldest available), 26 February 1991 |
| `822-31/` | Verordnung des Regierungsrates zum Bundesgesetz über die Heimarbeit (Heimarbeitsgesetz) (RB 822.31) | 1 | as enacted, 1 January 1984 |
| `823-20/` | Verordnung des Regierungsrates zur Bundesgesetzgebung über die in die Schweiz entsandten Arbeitnehmerinnen und Arbeitnehmer sowie zur Bundesgesetzgebung gegen die Schwarzarbeit (RB 823.20) | 1 | as enacted, 1 January 2008 |
| `831-10/` | Verordnung des Regierungsrates zum Einführungsgesetz über die Alters- und Hinterlassenenversicherung und über die Invalidenversicherung (RB 831.10) | 3 | oldest version available, then each consolidated version: 1 June 2004 to 1 June 2014 |
| `831-14-vkbv/` | Verordnung des Regierungsrates über die Verwaltungskostenbeiträge an die AHV/IV/EO/FL (RB 831.14) | 2 | oldest version available, then each consolidated version: 1 January 1993 to 1 January 2019 |
| `831-31-tg-elv/` | Verordnung zum Gesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (RB 831.31) | 11 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `831-411-gebr/` | Gebührenreglement (RB 831.411) | 4 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2026 |
| `832-10-tg-kvv/` | Krankenversicherungsverordnung (RB 832.10) | 20 | as enacted, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `832-12-vezl/` | Verordnung über die Einschränkung der Zulassung von Leistungserbringern und Leistungserbringerinnen zur Tätigkeit zulasten der obligatorischen Krankenpflegeversicherung (RB 832.12) | 4 | as enacted, then each consolidated version: 1 September 2013 to 1 February 2026 |
| `832-20/` | Verordnung des Regierungsrates zum Bundesgesetz vom 20. März 1981 über die Unfallversicherung (RB 832.20) | 1 | one version (the oldest available), 18 November 1997 |
| `836-11-tg-famzv/` | Familienzulagenverordnung (RB 836.11) | 7 | oldest version available, then each consolidated version: 1 January 2012 to 1 January 2026 |
| `836-21/` | Reglement der Familienausgleichskasse des Kantons Thurgau (RB 836.21) | 2 | oldest version available, then each consolidated version: 1 June 2004 to 1 June 2014 |
| `836-41-aliv/` | Alimentenhilfeverordnung (RB 836.41) | 2 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2022 |
| `837-11-masv/` | Verordnung über Massnahmen gegen die Arbeitslosigkeit und zur Standortförderung (RB 837.11) | 4 | oldest version available, then each consolidated version: 1 January 2006 to 1 April 2026 |
| `837-31-kassenreglement/` | Reglement des Regierungsrates über die Arbeitslosenkasse des Kantons Thurgau (RB 837.31) | 1 | one version (the oldest available), 18 November 1997 |
| `842-11/` | Verordnung des Regierungsrates zur Gesetzgebung über Massnahmen zur Förderung des Wohnungsbaues (RB 842.11) | 1 | as enacted, 15 May 1980 |
| `842-15/` | Verordnung des Regierungsrates zum Bundesgesetz über die Verbesserung der Wohnverhältnisse in Berggebieten (RB 842.15) | 1 | one version (the oldest available), 1 January 1998 |
| `850-11-shv/` | Sozialhilfeverordnung (RB 850.11) | 8 | oldest version available, then each consolidated version: 1 January 2013 to 1 January 2026 |
| `850-61-ivse-verordnung/` | Verordnung des Regierungsrates zur Interkantonalen Vereinbarung für soziale Einrichtungen (RB 850.61) | 1 | one version (the oldest available), 1 January 2013 |
| `850-71-hav/` | Heimaufsichtsverordnung (RB 850.71) | 3 | oldest version available, then each consolidated version: 1 January 2013 to 1 June 2023 |
| `910-11-lwv/` | Landwirtschaftsverordnung (RB 910.11) | 8 | oldest version available, then each consolidated version: 1 July 2010 to 1 August 2024 |
| `913-21-meliorationsverordnung-melv/` | Verordnung des Regierungsrates zum Gesetz über Bodenverbesserungen und landwirtschaftliche Hochbauten (RB 913.21) | 1 | one version (the oldest available), 6 May 2006 |
| `921-11-waldv/` | Waldverordnung (RB 921.11) | 3 | oldest version available, then each consolidated version: 1 January 2008 to 1 January 2026 |
| `921-13/` | Revierförsterverordnung (RB 921.13) | 3 | as enacted, then each consolidated version: 2 November 2013 to 1 January 2026 |
| `922-11-jgrv/` | Verordnung des Regierungsrates zum Gesetz über die Jagd und den Schutz wildlebender Säugetiere und Vögel (RB 922.11) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 April 2018 |
| `923-11-fiv/` | Fischereiverordnung (RB 923.11) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2023 |
| `923-421/` | Reglement des Departementes für Justiz und Sicherheit über die Verpachtung der Gemeindefischereirechte (RB 923.421) | 2 | oldest version available, then each consolidated version: 29 September 2001 to 1 January 2023 |
| `935-21-kspv/` | Kleinspielverordnung (RB 935.21) | 1 | as enacted, 1 January 2021 |
| `935-523-lfv/` | Lotteriefondsverordnung (RB 935.523) | 4 | oldest version available, then each consolidated version: 1 January 2006 to 1 June 2025 |
| `941-21/` | Verordnung des Regierungsrates über den Vollzug der Bundesgesetzgebung über das Messwesen (RB 941.21) | 2 | as enacted, then each consolidated version: 30 June 2007 to 1 December 2014 |
| `941-41/` | Verordnung des Regierungsrates zur eidgenössischen Sprengstoffgesetzgebung (RB 941.41) | 1 | one version (the oldest available), 1 January 2011 |
| `942-21/` | Verordnung des Regierungsrates betreffend die Anschrift der Detailpreise (RB 942.21) | 1 | one version (the oldest available), 1 January 2011 |
| `956-11/` | Reglement des Grossen Rates über die Organisation der Gebäudeversicherung des Kantons Thurgau (RB 956.11) | 1 | one version (the oldest available), 9 May 1983 |
| `956-12/` | Reglement des Verwaltungsrates über die Versicherungsbedingungen der Gebäudeversicherung (RB 956.12) | 1 | one version (the oldest available), 1 January 1989 |
| `956-13/` | Schätzungsverordnung des Verwaltungsrates der Gebäudeversicherung (RB 956.13) | 1 | one version (the oldest available), 1 January 2012 |
| `956-21/` | Reglement des Verwaltungsrates der Gebäudeversicherung über die Abgrenzung von Gebäude und Fahrhabe (RB 956.21) | 1 | as enacted, 1 January 2012 |
| `956-121/` | Geschäftsreglement der Gebäudeversicherung des Kantons Thurgau (RB 956.121) | 1 | one version (the oldest available), 1 January 2012 |

## Source

The RB (systematic collection) of the canton, published by the canton at <https://www.rechtsbuch.tg.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (ABl). Annexes the collection publishes only as separate PDF files are not included.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

`<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. One paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the canton's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (ABl), with an e-mail address that cannot exist (`<act key>@www.rechtsbuch.tg.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the canton publishes as binding (its chronological collection, or its systematic collection where cantonal law makes that binding). The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
