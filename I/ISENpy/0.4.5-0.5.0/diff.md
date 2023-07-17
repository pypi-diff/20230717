# Comparing `tmp/ISENpy-0.4.5.tar.gz` & `tmp/ISENpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ISENpy-0.4.5.tar", last modified: Thu Jun 29 20:57:15 2023, max compression
+gzip compressed data, was "ISENpy-0.5.0.tar", last modified: Mon Jul 17 19:43:02 2023, max compression
```

## Comparing `ISENpy-0.4.5.tar` & `ISENpy-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 20:57:15.179877 ISENpy-0.4.5/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 20:57:15.178765 ISENpy-0.4.5/ISENpy/
--rwxr-xr-x   0 corentin   (501) staff       (20)     1343 2023-06-29 20:56:26.000000 ISENpy-0.4.5/ISENpy/__init__.py
--rwxr-xr-x   0 corentin   (501) staff       (20)     7083 2023-06-29 10:44:46.000000 ISENpy-0.4.5/ISENpy/client.py
--rwxr-xr-x   0 corentin   (501) staff       (20)    30381 2023-06-29 16:35:56.000000 ISENpy-0.4.5/ISENpy/dataClasses.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 20:57:15.179607 ISENpy-0.4.5/ISENpy.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     5432 2023-06-29 20:57:15.000000 ISENpy-0.4.5/ISENpy.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      233 2023-06-29 20:57:15.000000 ISENpy-0.4.5/ISENpy.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-06-29 20:57:15.000000 ISENpy-0.4.5/ISENpy.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       18 2023-06-29 20:57:15.000000 ISENpy-0.4.5/ISENpy.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)        7 2023-06-29 20:57:15.000000 ISENpy-0.4.5/ISENpy.egg-info/top_level.txt
--rwxr-xr-x   0 corentin   (501) staff       (20)     1073 2023-06-29 20:56:05.000000 ISENpy-0.4.5/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     5432 2023-06-29 20:57:15.179765 ISENpy-0.4.5/PKG-INFO
--rwxr-xr-x   0 corentin   (501) staff       (20)     4996 2023-06-29 20:56:05.000000 ISENpy-0.4.5/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-06-29 20:57:15.179911 ISENpy-0.4.5/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      848 2023-06-29 20:56:23.000000 ISENpy-0.4.5/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-07-17 19:43:02.826085 ISENpy-0.5.0/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-07-17 19:43:02.825117 ISENpy-0.5.0/ISENpy/
+-rwxr-xr-x   0 corentin   (501) staff       (20)     1372 2023-07-17 19:41:01.000000 ISENpy-0.5.0/ISENpy/__init__.py
+-rw-r--r--   0 corentin   (501) staff       (20)     9558 2023-07-17 19:33:33.000000 ISENpy-0.5.0/ISENpy/classification.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)     8878 2023-07-17 19:39:55.000000 ISENpy-0.5.0/ISENpy/client.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)    32748 2023-07-17 19:23:09.000000 ISENpy-0.5.0/ISENpy/dataClasses.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-07-17 19:43:02.825695 ISENpy-0.5.0/ISENpy.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     7349 2023-07-17 19:43:02.000000 ISENpy-0.5.0/ISENpy.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      258 2023-07-17 19:43:02.000000 ISENpy-0.5.0/ISENpy.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-07-17 19:43:02.000000 ISENpy-0.5.0/ISENpy.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       18 2023-07-17 19:43:02.000000 ISENpy-0.5.0/ISENpy.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        7 2023-07-17 19:43:02.000000 ISENpy-0.5.0/ISENpy.egg-info/top_level.txt
+-rwxr-xr-x   0 corentin   (501) staff       (20)     1073 2023-06-29 20:56:05.000000 ISENpy-0.5.0/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     7349 2023-07-17 19:43:02.825948 ISENpy-0.5.0/PKG-INFO
+-rwxr-xr-x   0 corentin   (501) staff       (20)     6913 2023-07-17 19:36:32.000000 ISENpy-0.5.0/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-07-17 19:43:02.826126 ISENpy-0.5.0/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      848 2023-07-17 19:41:08.000000 ISENpy-0.5.0/setup.py
```

### Comparing `ISENpy-0.4.5/ISENpy/__init__.py` & `ISENpy-0.5.0/ISENpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 """
 
 
 __title__ = "ISENpy"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.4.5"
+__version__ = "0.5.0"
 
 
 from .dataClasses import *
 from .client import *
+from .classification import *
```

### Comparing `ISENpy-0.4.5/ISENpy/client.py` & `ISENpy-0.5.0/ISENpy/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+# client.py
+
+"""
+This file defines the ISEN class, which is the main class of the package.
+"""
+
 import requests
 from bs4 import BeautifulSoup
 import base64
 import json
 
 # IMPORT
 from . import dataClasses
+from . import classification
 
 
 class ISEN:
     """
     A ISEN-OUEST client.
     Parameters
     ----------
@@ -20,31 +27,58 @@
     ----------
     logged_in : bool
         If the user is successfully logged in
     username : str
     password : str
     Functions
     ----------
-    classMember(cycle:str, annee:str, ville:str) -> dict
+    classMember(cycle:str, annee:str, ville:str) -> classification.ClassMemberReport:
+        Parameters:
+            cycle: str "CIR", "CBIO", "CENT", "CEST", "CBIAST", "CSI"
+            annee: str "1", "2", "3"
+            ville: str "Caen", "Brest", "Nantes", "Rennes"
+        Return:
+            The class member
+                you can get value with a dict like this : classMember["nbMembers"] or classMember["data"][0]["name"]
+                or like this :  classMember.nbMembers or classMember.data[0].name
+    
     webAurion() -> dataClasses.WebAurion
-        grades() -> dict of grades of the user
-        absences() -> list of dict of absences of the user
-        planning() -> list of dict of planning of the user
-            start_date:str Optional -> The start of the planning (format : "dd-mm-yyyy")
-            end_end:str Optional -> The end of the planning  (format : "dd-mm-yyyy")
-
-        getOtherPlanning() -> list of dict of planning of the user
-            start_date:str Optional -> The start of the planning (format : "dd-mm-yyyy")
-            end_end:str Optional -> The end of the planning  (format : "dd-mm-yyyy")
-            classPlanning:str -> The class planning you want to get (Default: "CIR")
-            classCity:str -> The class city you want to get (Default: "Caen")
-            classYear:str -> The class year you want to get (Default: "1")
-            classGroup:str -> The class group you want to get (Default: "CBIO1 CIR1 Caen 2022-2023 Groupe 1")
+        grades() -> classification.GradeReport:
+            Return a dict with all the grades of the user and the average of the grades
+                you can get value with a dict like this : grades["average"] or grades["data"][0]["date"]
+                or like this :  grades.average or grades.data[0].date
+
+        absences() -> classification.AbsenceReport:
+            Return a list of dict of absences of the user
+                you can get value with a dict like this : absences["nbAbsences"] or absences["data"][0]["date"]
+                or like this :  absences.nbAbsences or absences.data[0].date
+
+        planning() -> classification.PlanningReport:
+            Parameters:
+                start_date : str, optional
+                    The start of the planning (format: "dd-mm-yyyy")
+                end_date : str, optional
+                    The end of the planning (format: "dd-mm-yyyy")
+            Return a list of dict of planning of the user
+                you can get value with a dict like this : planning["data"][0]["subject"] or planning["data"][0]["start"]
+                or like this :  planning.data[0].subject or planning.data[0].start
+
+        getOtherPlanning() -> classification.PlanningReport:
+            Parameters:
+                start_date:str Optional -> The start of the planning (format : "dd-mm-yyyy")
+                end_end:str Optional -> The end of the planning  (format : "dd-mm-yyyy")
+                classPlanning:str -> The class planning you want to get (Default: "CIR")
+                classCity:str -> The class city you want to get (Default: "Caen")
+                classYear:str -> The class year you want to get (Default: "1")
+                classGroup:str -> The class group you want to get (Default: "CBIO1 CIR1 Caen 2022-2023 Groupe 1")
+            Return a list of dict of planning of the class
+                you can get value with a dict like this : planning["data"][0]["subject"] or planning["data"][0]["start"]
+                or like this :  planning.data[0].subject or planning.data[0].start
 
-        getSchoolReport() -> dict of school report of the user (format : {"nbReport": int, "data": {"name": "id"}})
+        getSchoolReport() -> dict of school report of the user (format : {"nbReport": int, "data": [{"name": "id"}, ...]})
 
         downloadReport() -> Download the school report
             path (str, optional): path of the report. Defaults to the name in WebAurion.
             idReport (str, optional): id of the report. Defaults all the report of the user
 
 
     moodle() -> dataClasses.Moodle
@@ -144,20 +178,20 @@
     def moodle(self):
         """
         Return moodle informations
         """
         # Get the moodle informations file: "dataClasses.py"
         return dataClasses.Moodle(self.session)
 
-    def classMember(self, cycle: str, annee: str, ville: str) -> dict:
+    def classMember(self, cycle: str, annee: str, ville: str) -> classification.ClassMemberReport:
         """
         Args:
-            cycle:str "CIR", "CBIO", "CENT", "CEST", "CBIAST", "CSI"
-            annee:str "1", "2", "3"
-            ville:str "Caen", "Brest", "Nantes", "Rennes"
+            cycle: str "CIR", "CBIO", "CENT", "CEST", "CBIAST", "CSI"
+            annee: str "1", "2", "3"
+            ville: str "Caen", "Brest", "Nantes", "Rennes"
 
         Return:
             The class member
         """
 
         # Base url of trombinoscope
         baseUrl = "https://web.isen-ouest.fr/trombino"
@@ -179,29 +213,25 @@
         # Get the class member
         self.session.get(baseUrl)
         req = self.session.post(
             f"{baseUrl}/fonctions/ajax/lister_etudiants.php", data=payload
         )
         soup = BeautifulSoup(req.text, "html.parser")
         eleves = soup.find_all("td", {"id": "tdTrombi"})
-        # Create the dict of eleves
-        result = {
-            "nbEleves": len(eleves),
-            "data": [
-                {
-                    "nom": eleve.find("b").text,
-                    "mail": eleve.find("a").text,
-                    "avatarUrl": (baseUrl + eleve.find("img")["src"]).replace(
-                        " ./", "/"
-                    ),
-                }
-                for eleve in eleves
-            ],
-        }
-        # Return the dict of eleves
+        # Create the list of ClassMember objects
+        result = classification.ClassMemberReport(nbMembers=len(eleves), data=[])
+
+        for eleve in eleves:
+            name = eleve.find("b").text
+            mail = eleve.find("a").text
+            avatar_url = (baseUrl + eleve.find("img")["src"]).replace(" ./", "/")
+            class_member = classification.ClassMember(name=name, mail=mail, avatar_url=avatar_url)
+            result.data.append(class_member)
+
+        # Return the ClassMemberReport object
         return result
 
     def userInfo(self) -> dict:
         """
         Return your user info
         """
```

### Comparing `ISENpy-0.4.5/ISENpy/dataClasses.py` & `ISENpy-0.5.0/ISENpy/dataClasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+# dataClasses.py
+
+"""
+This file defines classes to represent WebAurion, Moodle, and their respective data
+"""
+
 from typing import Optional
 import requests
 from bs4 import BeautifulSoup
 import json
 import datetime
 
+# IMPORT 
+from . import classification
+
 class WebAurion:
     """
     WebAurion Information
 
     Parameters
     ----------
     session : requests.Session
@@ -16,26 +25,33 @@
     Attributes
     ----------
     session : requests.Session
         The session of the user
 
     Functions
     ----------
-    grades() -> dict:
-        Return a dict with all the grades of the user
+    grades() -> classification.GradeReport:
+        Return a dict with all the grades of the user and the average of the grades
+            you can get value with a dict like this : grades["average"] or grades["data"][0]["date"]
+            or like this :  grades.average or grades.data[0].date
 
-    absences() -> list:
+    absences() -> classification.AbsenceReport:
         Return a list of dict of absences of the user
+            you can get value with a dict like this : absences["nbAbsences"] or absences["data"][0]["date"]
+            or like this :  absences.nbAbsences or absences.data[0].date
 
-    planning() -> list:
+    planning() -> classification.PlanningReport:
+        Parameters:
+            start_date : str, optional
+                The start of the planning (format: "dd-mm-yyyy")
+            end_date : str, optional
+                The end of the planning (format: "dd-mm-yyyy")
         Return a list of dict of planning of the user
-        start_date : str, optional
-            The start of the planning (format: "dd-mm-yyyy")
-        end_date : str, optional
-            The end of the planning (format: "dd-mm-yyyy")
+            you can get value with a dict like this : planning["data"][0]["subject"] or planning["data"][0]["start"]
+            or like this :  planning.data[0].subject or planning.data[0].start
 
     otherPlanning() -> list:
         Return a list of dict of planning of the user
         start_date : str, optional
             The start of the planning (format: "dd-mm-yyyy")
         end_date : str, optional
             The end of the planning (format: "dd-mm-yyyy")
@@ -68,16 +84,18 @@
         classPlanning : str, optional
             The class of the planning (Ex.: "CIR")
         classCity : str, optional
             The city of the planning (Ex.: "Caen")
         classYear : str, optional
             The year of the planning (Ex.: "1")
 
-    getSchoolReport() -> dict:
-        Return a dict of the user's report
+    getSchoolReport() -> classification.SchoolReport:
+        Return a dict of the user's report (format: {"nbReports": int, "data": [{"name": "id"}, ...]})
+            you can get value with a dict like this : report["nbReports"] or report["data"][0]["name"]
+            or like this :  report.nbReport or report.data[0].name or report.data[0].id
 
     downloadReport() -> None:
         Download the user's report
         path : str, optional
             The path of the report (Default: the name of the file in WebAurion)
         idReport : str, optional
             The id of the report (Default: all the user's reports)
@@ -150,80 +168,94 @@
                 value = ""
             else:
                 value = i["value"]
             payload2[i["name"]] = value
 
         return payload2
 
-    def grades(self) -> dict:
+
+    def grades(self) -> classification.GradeReport:
+        # Get the grades page
         gradeUrl = "https://web.isen-ouest.fr/webAurion/faces/LearnerNotationListPage.xhtml"
+        # Set the payload
         payload = self.payloadForGrades
         pageGrade = self.__webAurion(gradeUrl, payload)
+        # Scrap the page to get information about the grades
         soup = BeautifulSoup(pageGrade.text, "html.parser")
         result = soup.find_all("tr")[1:]
-        gradeInfo = {"gradeAverage": "", "data": []}
+        # Set the list of dict of the grades
+        grades = []
+        grade_sum = 0
+        grade_count = 0
+
+        # Check if the user does not have any grades
         for tr in result:
-            gradeInfo["data"].append({
-                "date": tr.find_all("td")[0].text,
-                "code": tr.find_all("td")[1].text,
-                "nom": tr.find_all("td")[2].text,
-                "note": tr.find_all("td")[3].text,
-                "abs": tr.find_all("td")[4].text,
-                "appreciation": tr.find_all("td")[5].text,
-                "intervenants": tr.find_all("td")[6].text
-            })
-        gradeAverage = 0
-        noGrade = 0
-        for grade in gradeInfo["data"]:
-            if grade["note"] != "" and grade["note"] != "-":
-                gradeAverage += float(grade["note"])
-            else:
-                noGrade += 1
-        gradeInfo["gradeAverage"] = round(gradeAverage / (len(gradeInfo["data"]) - noGrade), 2)
-        return gradeInfo
+            date, code, name, grade, absence, appreciation, instructors = (td.text for td in tr.find_all("td"))
+            if grade != "" and grade != "-":
+                grade_sum += float(grade)
+                grade_count += 1
+
+            # Set the dict of the grade
+            note = classification.Grade(date=date, code=code, name=name, grade=grade, absence=absence, appreciation=appreciation, instructors=instructors)
+            grades.append(note)
+            
+        # Set the average of the grades
+        grade_average = round(grade_sum / grade_count, 2) if grade_count > 0 else 0
+        grade_report = classification.GradeReport(grade_average=grade_average, grades=grades)
+
+        # Return the dict of the grades
+        return grade_report
+
 
-    def absences(self) -> dict:
-        """
-        Return a dictionary with all the absences of the user
-        """
 
-        # Url of the absences page
-        absencesUrl = "https://web.isen-ouest.fr/webAurion/faces/MesAbsences.xhtml"
+    def absences(self) -> classification.AbsenceReport:
+        # Get the absences page
+        absences_url = "https://web.isen-ouest.fr/webAurion/faces/MesAbsences.xhtml"
         # Set the payload
         payload = self.payloadForAbsences
-        pageAbsences = self.__webAurion(absencesUrl, payload)
+        absences_page = self.__webAurion(absences_url, payload)
         # Scrap the page to get information about the absences
-        soup = BeautifulSoup(pageAbsences.text, "html.parser")
-        checkAbs = soup.find_all("tr")[6:]
+        soup = BeautifulSoup(absences_page.text, "html.parser")
+        # Check if the user does not have any absences
+        check_absences = soup.find_all("tr")[6:]
         result = soup.find_all("tbody")[1].find_all("tr")
         total = soup.find_all("tbody")[2].find_all("tr")
-        
-        # If the user does not have any absence
-        if len(result) == 1 and checkAbs[0].find_all("td")[0].text == "Aucune absence.":
-            return {"nbAbsences": "0", "time": "0", "data": []}
 
-        absencesInfo = {"nbAbsences": "", "data": []}
+        # Set the list of dict of the absences
+        if len(result) == 1 and check_absences[0].find_all("td")[0].text == "Aucune absence.":
+            return classification.AbsenceReport(nbAbsences="0", time="0", data=[])
+
+        # Set the dict of the absences
+        absences_info = {"nbAbsences": "", "absences": []}
         for tr in result:
-            absencesInfo["data"].append({
+            absences_info["absences"].append({
                 "date": tr.find_all("td")[0].text,
-                "motif": tr.find_all("td")[1].text,
-                "duree": tr.find_all("td")[2].text,
-                "horaire": tr.find_all("td")[3].text,
-                "cours": tr.find_all("td")[4].text,
-                "intervenant": tr.find_all("td")[5].text,
-                "matiere": tr.find_all("td")[6].text
+                "reason": tr.find_all("td")[1].text,
+                "duration": tr.find_all("td")[2].text,
+                "schedule": tr.find_all("td")[3].text,
+                "course": tr.find_all("td")[4].text,
+                "instructor": tr.find_all("td")[5].text,
+                "subject": tr.find_all("td")[6].text
             })
-        absencesInfo["nbAbsences"] = total[0].find_all("td")[1].text
-        absencesInfo["time"] = total[1].find_all("td")[1].text
-        # Return the dictionary of absences
+        absences_info["nbAbsences"] = total[0].find_all("td")[1].text
+        absences_info["time"] = total[1].find_all("td")[1].text
+
+        # Return the dict of the absences
+        absences_data = absences_info["absences"]
+        data = [classification.Absence(date=a["date"], reason=a["reason"], duration=a["duration"], schedule=a["schedule"],
+                        course=a["course"], instructor=a["instructor"], subject=a["subject"])
+                    for a in absences_data]
+
+        # Set the dict of the absences
+        absencesInfo = classification.AbsenceReport(nbAbsences=absences_info["nbAbsences"], time=absences_info["time"], data=data)
         return absencesInfo
 
 
     def __getWorkingTime(self, req: requests.get, start_date: str = None, end_date: str = None,
-                        isOtherPlanning: bool = False, classe: str = "") -> list:
+                        isOtherPlanning: bool = False, classe: str = "") -> classification.PlanningReport:
         """ Get the working time of the user
 
         Args:
             req (requests.get): request of the page
             start_date (str, optional): the start date of the planning. Defaults to None.
             end_date (str, optional): the end date of the planning. Defaults to None.
             isOtherPlanning (bool, optional): if the planning is for another user. Defaults to False.
@@ -274,40 +306,42 @@
             raise Exception("Error while parsing the planning")
 
         # Set the workingTime list for the week
         workingTime = []
 
         for i in planning["events"]:
             info = i["title"].split(" - ")
-            planning_data = {
+            event_data = {
                 "id": i["id"],
                 "start": i["start"],
                 "end": i["end"],
-                "className": i["className"],
+                "class_name": i["className"],
                 "type": info[2],
-                "matiere": info[3] if i["className"] != "DS" else ", ".join(info[4:-3]),
+                "subject": info[3] if i["className"] != "DS" else ", ".join(info[4:-3]),
                 "description": ", ".join(info[4:-2]) if i["className"] != "DS" else ", ".join(info[4:-3]),
-                "intervenants": info[-2]
+                "instructors": info[-2]
             }
 
             if isOtherPlanning:
-                planning_data["debut"] = info[0]
-                planning_data["fin"] = info[1]
-                planning_data["salle"] = info[-1]
-                planning_data["classe"] = classe
+                event_data["start_time"] = info[0]
+                event_data["end_time"] = info[1]
+                event_data["room"] = info[-1]
+                event_data["class_info"] = classe
             else:
-                planning_data["debut"] = info[0].split(" à ")[0]
-                planning_data["fin"] = info[0].split(" à ")[1]
-                planning_data["salle"] = info[1]
-                planning_data["classe"] = info[-1]
-
-            workingTime.append(planning_data)
-
-        # Return the list of dict of the planning
-        return workingTime
+                event_data["start_time"] = info[0].split(" à ")[0]
+                event_data["end_time"] = info[0].split(" à ")[1]
+                event_data["room"] = info[1]
+                event_data["class_info"] = info[-1]
+
+            event_obj = classification.Event(**event_data) # ** is for splited dict to args of the class 'Event'
+            workingTime.append(event_obj)
+
+        # get the planning report
+        planning_report = classification.PlanningReport(events=workingTime)
+        return planning_report
 
 
     def planning(self, start_date: Optional[str] = None, end_date: Optional[str] = None) -> list:
         """
         Args:
             start (str, optional): The start date of the planning. Defaults to None. (Format : "dd-mm-yyyy")
             end (str, optional): The end date of the planning. Defaults to None. (Format : "dd-mm-yyyy")
@@ -508,20 +542,21 @@
         payloadForChoicePlanning = {classYear: self.__getPayloadOfThePage(self.classPlanning[classPlanning]["city"][classCity]["year"][classYear]["extraInfo"].text)}
         payloadForChoicePlanning[classYear].update(lastPayload)
 
         req = self.session.post("https://web.isen-ouest.fr/webAurion/faces/ChoixPlanning.xhtml", data=payloadForChoicePlanning[classYear])
 
         return self.__getWorkingTime(req, start_date, end_date, True, classGroup)
 
-    def getSchoolReport(self) -> dict:
-        """Get the report of the user
+    def getSchoolReport(self) -> classification.SchoolReport:
+        """
+        Get the report of the user
 
         Returns:
             dict: Dictionary containing the report information.
-                Format: {"nbReport": int, "data": {"name": "id"}}
+                Format: {"num_reports": int, "data": [{"name": "id"}, ...]}
 
         Raises:
             Exception: If the user does not have any report.
         """
 
         urlPost = self.baseMainPageUrl
 
@@ -567,23 +602,27 @@
 
         self.payloadReport = self.__getPayloadOfThePage(req.text)
 
         soup = BeautifulSoup(req.text, "html.parser")
 
         report = soup.find("div", {"class": "ui-datatable-tablewrapper"}).find("select").find_all("option")
 
-        result = {"nbReport": len(report), "data": []}
+        result = {"nbReports": len(report), "data": []}
 
         for i in report:
             nameFile = i.text.split(".pdf")[0].strip() + ".pdf"
-            result["data"].append({"name": nameFile, "id": i["value"]})
+            report_data = classification.SchoolReportData(name=nameFile, id=i["value"])
+            result["data"].append(report_data)
+        
+        schoolReport = classification.SchoolReport(**result)
+        
+        self.infoReport = schoolReport
 
-        self.infoReport = result
+        return schoolReport
 
-        return result
 
 
     def downloadReport(self, path: str = None, idReport: str = None) -> None:
         """Download the report of the user
 
         Args:
             path (str, optional): Path of the report. Defaults to the name in WebAurion.
@@ -593,34 +632,36 @@
             Exception: If the user does not have any report.
             Exception: If the report is not found.
         """
 
         if not self.payloadReport:
             self.infoReport = self.getSchoolReport()
 
-        if self.infoReport["nbReport"] == 0:
+        if self.infoReport.nbReports == 0:
             raise Exception("The user does not have any report")
 
-        if self.infoReport["nbReport"] > 1 and path is not None:
-            raise Exception("The user has more than one report. Please choose either no path or no specific path.")
+        if self.infoReport.nbReports > 1 and path is None and idReport is None:
+            for report in self.infoReport.data:
+                self.downloadReport(path=report.name, idReport=report.id)
+            return
 
         if path is None and idReport is not None:
-            # self.infoReport format : {"nbReport": int, "data":  ({"name": "name", "id":"id"}, ...)}]}
-            for i in self.infoReport["data"]:
-                if i["id"] == idReport:
-                    path = i["name"]
+            # self.infoReport format : {"nbReports": int, "data":  ({"name": "name", "id":"id"}, ...)}]}
+            for i in self.infoReport.data:
+                if i.id == idReport:
+                    path = i.name
                     break
             if path is None:
                 raise Exception("The report is not found")
 
         if idReport is None:
-            for i in self.infoReport["data"]:
+            for i in self.infoReport.data:
                 if path is None:
-                    path = i["name"]
-                self.downloadReport(path=i["name"], idReport=i["id"])
+                    path = i.name
+                self.downloadReport(path=i.name, idReport=i.id)
                 return
 
         urlChoixDonnee = "https://web.isen-ouest.fr/webAurion/faces/ChoixDonnee.xhtml"
 
         payload = {
             'form:j_idt193:0:j_idt209': 'form:j_idt193:0:j_idt209',
             "form:j_idt193:0:documents_input": idReport,
@@ -629,14 +670,17 @@
         payload.update(self.payloadReport)
 
         req = self.session.post(urlChoixDonnee, data=payload)
 
         if req.status_code != 200:
             raise Exception(f"WebAuiron is not available at the moment: Error {req.status_code}")
 
+        if not path.endswith(".pdf"):
+            path += ".pdf"
+        
         with open(path, "wb") as f:
             f.write(req.content)
 
             
 
 class Moodle:
     """Class to get the resources of the user's courses. (on Moodle)
```

### Comparing `ISENpy-0.4.5/ISENpy.egg-info/PKG-INFO` & `ISENpy-0.5.0/ISENpy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.5
+Version: 0.5.0
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,15 @@
 - requests
 - bs4
 - lxml
 
 ## Usage
 
 
-- `pip3 install ISENpy`
+- `pip3 install ISENpy -U`
 
 Here is an example script:
 
 ```python
 import ISENpy
 
 # Create a new instance of the ISENpy class
@@ -58,36 +58,138 @@
 #Check if the user is logged in
 if not client.logged_in:
     print("Identifiant ou mot de passe incorect !!")
     exit()
 
 #Example of use
 classMember = client.classMember("CIR", "1", "Caen") #Get all the students of the class CIR1 Caen
-print(classMember)
+print(f"nb of member : {classMember.nbMembers}")
+for student in classMember.data:
+    print(f"{student.name} | {student.mail} | {student.avatar_url}")
+
+# or more simply
+
+# print(classMember)
+# print(f"nb of member : {classMember['nbMembers']}")
+# for student in classMember['data']:
+#     print(f"{student['name']} | {student['mail']} | {student['avatar_url']}")
+
 
 userInfo = client.userInfo() #Get your user info
 print(userInfo) 
 
-#Get the webAurion object
+```
+
+## Example for get your grades
+
+```python
+
+...
+
 webAurion = client.webAurion()
 
-absence = webAurion.absences() #Get your absences
-print(absence)
+grades = webAurion.grades()
 
-grade = webAurion.grades() #Get your grades
-print(grade)
+print(grades.average)
+for grade in grades.data:
+    print(f"{grade.date} : {grade.grade} ({grade.name} | {grade.instructors}), {grade.appreciation}, {grade.absence}")
 
-planning = webAurion.planning() #Get your planning of the week. Argument(Optional) : 'start_date' (format : "dd-mm-yyyy") and 'end_date' (format : "dd-mm-yyyy")
-print(planning)
+# Or more simply
+
+# print(grades)
+# print(grades["data"][0]["date"]) # ... (use like a dict)
+
+```
+
+## Example for get your absences
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+absences = webAurion.absences()
+
+print(absences.nbAbsences)
+print(absences.time)
+for absence in absences.data:
+    print(f" \
+            {absence.date} : {absence.reason} \
+            ({absence.duration} | {absence.schedule} | {absence.course} | \
+            {absence.instructor} | {absence.subject}) \
+        ")
+    
+# Or more simply
+
+# print(absences)
+# print(absences["data"][0]["date"]) # ... (use like a dict)
+
+```
+
+## Example for get your planning
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+planning = webAurion.planning()
+
+for event in planning.data:
+    print(f" \
+            {event.subject} ({event.start} | {event.end} , \
+            {event.start_time} | {event.end_time},  {event.instructor} | {event.room}), \
+            {event.type}, {event.class_name}, {event.description}, {event.class_info} \
+        ")
+    
+# Or more simply
+
+# print(planning)
+# print(planning["data"][0]["subject"]) # ... (use like a dict)
+
+```
+
+## Example for get your shool report
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+schoolReport = webAurion.getSchoolReport()
+
+print(schoolReport.nbReports)
+for report in schoolReport.data:
+    print(f"{report.name} : {report.id}")
+
+# Or more simply
+
+# print(schoolReport)
+# print(schoolReport["data"][0]["name"]) # ... (use like a dict)
+
+
+```
+
+## And for download your school report
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+webAurion.downloadReport() #Download all your school report with the default name
 
-schoolReport = webAurion.getSchoolReport() #Get your school report
-print(schoolReport)
+# if you want only one report
 
-# for download the report
-#webAurion.downloadReport() #Download the school report. Argument(Optional) : 'path' (format : "path/to/file.pdf") and 'idReport' (format : "id")
+# webAurion.downloadReport(idReport="report_id") 
+# Download the report with the id "report_id" with the default name (you have the id with the schoolReport object Ex. schoolReport = webAurion.getSchoolReport() ) 
 
 ```
 
 ## Other example if you  want to get your planning in the calendar of your computer
 
 - This script uses the 'ics' and 'datetime' modules
 - `pip3 install ics datetime`
@@ -109,21 +211,21 @@
 
 webAurion = client.webAurion() #Get the webAurion object
 
 planning = webAurion.planning() #Get your planning of the week. Argument(Optional) : 'start_date' (format : "dd-mm-yyyy") and 'end_date' (format : "dd-mm-yyyy")
 
 c = Calendar()
 
-for i in planning:
+for event in planning.data:
     e = Event()
-    e.name = i["matiere"] + " - " + i["type"]
-    e.description = i["description"] + " - intervenants: " + i["intervenants"] + " - classe: " + i["classe"]
-    e.location = i["salle"]
-    e.begin = datetime.fromisoformat(i["start"][:-2] + ':00')
-    e.end = datetime.fromisoformat(i["end"][:-2] + ':00')
+    e.name = event.subject + " - " + event.type
+    e.description = event.description + " - intervenants: " + event.instructor + " - classe: " + event.class_name
+    e.location = event.room
+    e.begin = datetime.fromisoformat(event.start[:-2] + ':00')
+    e.end = datetime.fromisoformat(event.end[:-2] + ':00')
     c.events.add(e)
 
 with open('week.ics', 'w') as my_file:
     my_file.writelines(c.serialize_iter())
 
 ```
```

### Comparing `ISENpy-0.4.5/LICENSE` & `ISENpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.5/PKG-INFO` & `ISENpy-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.5
+Version: 0.5.0
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,15 @@
 - requests
 - bs4
 - lxml
 
 ## Usage
 
 
-- `pip3 install ISENpy`
+- `pip3 install ISENpy -U`
 
 Here is an example script:
 
 ```python
 import ISENpy
 
 # Create a new instance of the ISENpy class
@@ -58,36 +58,138 @@
 #Check if the user is logged in
 if not client.logged_in:
     print("Identifiant ou mot de passe incorect !!")
     exit()
 
 #Example of use
 classMember = client.classMember("CIR", "1", "Caen") #Get all the students of the class CIR1 Caen
-print(classMember)
+print(f"nb of member : {classMember.nbMembers}")
+for student in classMember.data:
+    print(f"{student.name} | {student.mail} | {student.avatar_url}")
+
+# or more simply
+
+# print(classMember)
+# print(f"nb of member : {classMember['nbMembers']}")
+# for student in classMember['data']:
+#     print(f"{student['name']} | {student['mail']} | {student['avatar_url']}")
+
 
 userInfo = client.userInfo() #Get your user info
 print(userInfo) 
 
-#Get the webAurion object
+```
+
+## Example for get your grades
+
+```python
+
+...
+
 webAurion = client.webAurion()
 
-absence = webAurion.absences() #Get your absences
-print(absence)
+grades = webAurion.grades()
 
-grade = webAurion.grades() #Get your grades
-print(grade)
+print(grades.average)
+for grade in grades.data:
+    print(f"{grade.date} : {grade.grade} ({grade.name} | {grade.instructors}), {grade.appreciation}, {grade.absence}")
 
-planning = webAurion.planning() #Get your planning of the week. Argument(Optional) : 'start_date' (format : "dd-mm-yyyy") and 'end_date' (format : "dd-mm-yyyy")
-print(planning)
+# Or more simply
+
+# print(grades)
+# print(grades["data"][0]["date"]) # ... (use like a dict)
+
+```
+
+## Example for get your absences
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+absences = webAurion.absences()
+
+print(absences.nbAbsences)
+print(absences.time)
+for absence in absences.data:
+    print(f" \
+            {absence.date} : {absence.reason} \
+            ({absence.duration} | {absence.schedule} | {absence.course} | \
+            {absence.instructor} | {absence.subject}) \
+        ")
+    
+# Or more simply
+
+# print(absences)
+# print(absences["data"][0]["date"]) # ... (use like a dict)
+
+```
+
+## Example for get your planning
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+planning = webAurion.planning()
+
+for event in planning.data:
+    print(f" \
+            {event.subject} ({event.start} | {event.end} , \
+            {event.start_time} | {event.end_time},  {event.instructor} | {event.room}), \
+            {event.type}, {event.class_name}, {event.description}, {event.class_info} \
+        ")
+    
+# Or more simply
+
+# print(planning)
+# print(planning["data"][0]["subject"]) # ... (use like a dict)
+
+```
+
+## Example for get your shool report
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+schoolReport = webAurion.getSchoolReport()
+
+print(schoolReport.nbReports)
+for report in schoolReport.data:
+    print(f"{report.name} : {report.id}")
+
+# Or more simply
+
+# print(schoolReport)
+# print(schoolReport["data"][0]["name"]) # ... (use like a dict)
+
+
+```
+
+## And for download your school report
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+webAurion.downloadReport() #Download all your school report with the default name
 
-schoolReport = webAurion.getSchoolReport() #Get your school report
-print(schoolReport)
+# if you want only one report
 
-# for download the report
-#webAurion.downloadReport() #Download the school report. Argument(Optional) : 'path' (format : "path/to/file.pdf") and 'idReport' (format : "id")
+# webAurion.downloadReport(idReport="report_id") 
+# Download the report with the id "report_id" with the default name (you have the id with the schoolReport object Ex. schoolReport = webAurion.getSchoolReport() ) 
 
 ```
 
 ## Other example if you  want to get your planning in the calendar of your computer
 
 - This script uses the 'ics' and 'datetime' modules
 - `pip3 install ics datetime`
@@ -109,21 +211,21 @@
 
 webAurion = client.webAurion() #Get the webAurion object
 
 planning = webAurion.planning() #Get your planning of the week. Argument(Optional) : 'start_date' (format : "dd-mm-yyyy") and 'end_date' (format : "dd-mm-yyyy")
 
 c = Calendar()
 
-for i in planning:
+for event in planning.data:
     e = Event()
-    e.name = i["matiere"] + " - " + i["type"]
-    e.description = i["description"] + " - intervenants: " + i["intervenants"] + " - classe: " + i["classe"]
-    e.location = i["salle"]
-    e.begin = datetime.fromisoformat(i["start"][:-2] + ':00')
-    e.end = datetime.fromisoformat(i["end"][:-2] + ':00')
+    e.name = event.subject + " - " + event.type
+    e.description = event.description + " - intervenants: " + event.instructor + " - classe: " + event.class_name
+    e.location = event.room
+    e.begin = datetime.fromisoformat(event.start[:-2] + ':00')
+    e.end = datetime.fromisoformat(event.end[:-2] + ':00')
     c.events.add(e)
 
 with open('week.ics', 'w') as my_file:
     my_file.writelines(c.serialize_iter())
 
 ```
```

### Comparing `ISENpy-0.4.5/README.md` & `ISENpy-0.5.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 - requests
 - bs4
 - lxml
 
 ## Usage
 
 
-- `pip3 install ISENpy`
+- `pip3 install ISENpy -U`
 
 Here is an example script:
 
 ```python
 import ISENpy
 
 # Create a new instance of the ISENpy class
@@ -44,36 +44,138 @@
 #Check if the user is logged in
 if not client.logged_in:
     print("Identifiant ou mot de passe incorect !!")
     exit()
 
 #Example of use
 classMember = client.classMember("CIR", "1", "Caen") #Get all the students of the class CIR1 Caen
-print(classMember)
+print(f"nb of member : {classMember.nbMembers}")
+for student in classMember.data:
+    print(f"{student.name} | {student.mail} | {student.avatar_url}")
+
+# or more simply
+
+# print(classMember)
+# print(f"nb of member : {classMember['nbMembers']}")
+# for student in classMember['data']:
+#     print(f"{student['name']} | {student['mail']} | {student['avatar_url']}")
+
 
 userInfo = client.userInfo() #Get your user info
 print(userInfo) 
 
-#Get the webAurion object
+```
+
+## Example for get your grades
+
+```python
+
+...
+
 webAurion = client.webAurion()
 
-absence = webAurion.absences() #Get your absences
-print(absence)
+grades = webAurion.grades()
 
-grade = webAurion.grades() #Get your grades
-print(grade)
+print(grades.average)
+for grade in grades.data:
+    print(f"{grade.date} : {grade.grade} ({grade.name} | {grade.instructors}), {grade.appreciation}, {grade.absence}")
 
-planning = webAurion.planning() #Get your planning of the week. Argument(Optional) : 'start_date' (format : "dd-mm-yyyy") and 'end_date' (format : "dd-mm-yyyy")
-print(planning)
+# Or more simply
+
+# print(grades)
+# print(grades["data"][0]["date"]) # ... (use like a dict)
+
+```
+
+## Example for get your absences
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+absences = webAurion.absences()
+
+print(absences.nbAbsences)
+print(absences.time)
+for absence in absences.data:
+    print(f" \
+            {absence.date} : {absence.reason} \
+            ({absence.duration} | {absence.schedule} | {absence.course} | \
+            {absence.instructor} | {absence.subject}) \
+        ")
+    
+# Or more simply
+
+# print(absences)
+# print(absences["data"][0]["date"]) # ... (use like a dict)
+
+```
+
+## Example for get your planning
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+planning = webAurion.planning()
+
+for event in planning.data:
+    print(f" \
+            {event.subject} ({event.start} | {event.end} , \
+            {event.start_time} | {event.end_time},  {event.instructor} | {event.room}), \
+            {event.type}, {event.class_name}, {event.description}, {event.class_info} \
+        ")
+    
+# Or more simply
+
+# print(planning)
+# print(planning["data"][0]["subject"]) # ... (use like a dict)
+
+```
+
+## Example for get your shool report
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+schoolReport = webAurion.getSchoolReport()
+
+print(schoolReport.nbReports)
+for report in schoolReport.data:
+    print(f"{report.name} : {report.id}")
+
+# Or more simply
+
+# print(schoolReport)
+# print(schoolReport["data"][0]["name"]) # ... (use like a dict)
+
+
+```
+
+## And for download your school report
+
+```python
+
+...
+
+webAurion = client.webAurion()
+
+webAurion.downloadReport() #Download all your school report with the default name
 
-schoolReport = webAurion.getSchoolReport() #Get your school report
-print(schoolReport)
+# if you want only one report
 
-# for download the report
-#webAurion.downloadReport() #Download the school report. Argument(Optional) : 'path' (format : "path/to/file.pdf") and 'idReport' (format : "id")
+# webAurion.downloadReport(idReport="report_id") 
+# Download the report with the id "report_id" with the default name (you have the id with the schoolReport object Ex. schoolReport = webAurion.getSchoolReport() ) 
 
 ```
 
 ## Other example if you  want to get your planning in the calendar of your computer
 
 - This script uses the 'ics' and 'datetime' modules
 - `pip3 install ics datetime`
@@ -95,21 +197,21 @@
 
 webAurion = client.webAurion() #Get the webAurion object
 
 planning = webAurion.planning() #Get your planning of the week. Argument(Optional) : 'start_date' (format : "dd-mm-yyyy") and 'end_date' (format : "dd-mm-yyyy")
 
 c = Calendar()
 
-for i in planning:
+for event in planning.data:
     e = Event()
-    e.name = i["matiere"] + " - " + i["type"]
-    e.description = i["description"] + " - intervenants: " + i["intervenants"] + " - classe: " + i["classe"]
-    e.location = i["salle"]
-    e.begin = datetime.fromisoformat(i["start"][:-2] + ':00')
-    e.end = datetime.fromisoformat(i["end"][:-2] + ':00')
+    e.name = event.subject + " - " + event.type
+    e.description = event.description + " - intervenants: " + event.instructor + " - classe: " + event.class_name
+    e.location = event.room
+    e.begin = datetime.fromisoformat(event.start[:-2] + ':00')
+    e.end = datetime.fromisoformat(event.end[:-2] + ':00')
     c.events.add(e)
 
 with open('week.ics', 'w') as my_file:
     my_file.writelines(c.serialize_iter())
 
 ```
```

### Comparing `ISENpy-0.4.5/setup.py` & `ISENpy-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ISENpy',
-    version='0.4.5',    
+    version='0.5.0',    
     description='A python API wrapper for ISEN-OUEST',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/ISENpy',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

