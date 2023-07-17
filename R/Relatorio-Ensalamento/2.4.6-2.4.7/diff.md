# Comparing `tmp/Relatorio_Ensalamento-2.4.6.tar.gz` & `tmp/Relatorio_Ensalamento-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Relatorio_Ensalamento-2.4.6.tar", last modified: Fri Jul 14 21:20:01 2023, max compression
+gzip compressed data, was "Relatorio_Ensalamento-2.4.7.tar", last modified: Mon Jul 17 20:50:20 2023, max compression
```

## Comparing `Relatorio_Ensalamento-2.4.6.tar` & `Relatorio_Ensalamento-2.4.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.443735 Relatorio_Ensalamento-2.4.6/
--rw-rw-rw-   0        0        0      549 2023-07-14 21:20:01.443735 Relatorio_Ensalamento-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.404283 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/
--rw-rw-rw-   0        0        0    50179 2023-07-14 20:55:33.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/Relatorio_Ensalamento.py
--rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.426481 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/
--rw-rw-rw-   0        0        0      549 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.434477 Relatorio_Ensalamento-2.4.6/Sugestao/
--rw-rw-rw-   0        0        0    59471 2023-07-14 21:19:02.000000 Relatorio_Ensalamento-2.4.6/Sugestao/Sugestao.py
--rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.6/Sugestao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.441689 Relatorio_Ensalamento-2.4.6/Unificar_XML/
--rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.6/Unificar_XML/Unificar_XML.py
--rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.6/Unificar_XML/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-14 21:20:01.448648 Relatorio_Ensalamento-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-07-14 21:19:58.000000 Relatorio_Ensalamento-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:50:20.785148 Relatorio_Ensalamento-2.4.7/
+-rw-rw-rw-   0        0        0      549 2023-07-17 20:50:20.786152 Relatorio_Ensalamento-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 20:50:20.734443 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento/
+-rw-rw-rw-   0        0        0    50189 2023-07-17 20:50:16.000000 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento/Relatorio_Ensalamento.py
+-rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:50:20.756723 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-07-17 20:50:20.000000 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-17 20:50:20.000000 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 20:50:20.000000 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-17 20:50:20.000000 Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 20:50:20.769956 Relatorio_Ensalamento-2.4.7/Sugestao/
+-rw-rw-rw-   0        0        0    59471 2023-07-14 21:19:02.000000 Relatorio_Ensalamento-2.4.7/Sugestao/Sugestao.py
+-rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.7/Sugestao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 20:50:20.783075 Relatorio_Ensalamento-2.4.7/Unificar_XML/
+-rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.7/Unificar_XML/Unificar_XML.py
+-rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.7/Unificar_XML/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-07-17 20:50:20.791149 Relatorio_Ensalamento-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-07-17 20:50:16.000000 Relatorio_Ensalamento-2.4.7/setup.py
```

### Comparing `Relatorio_Ensalamento-2.4.6/PKG-INFO` & `Relatorio_Ensalamento-2.4.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio_Ensalamento
-Version: 2.4.6
+Version: 2.4.7
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/Relatorio_Ensalamento.py` & `Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento/Relatorio_Ensalamento.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,45 +3,42 @@
 análise a respeito das vagas e das capacidades das salas. O script utiliza o XML Unificado do ASC (COA), o re-
 latório de capacidade (COA) e o excel de Carga Horária por Turma/Disciplina (Prime). Foi desenvolvido uma tela
 para a seleção dos arquivos utilizados. O código é utilizado atualmente pela equipe da CIA
 
 
 Desenvolvido por Matheus Rosa e Fernando Dias
 '''
-
-import time
+from datetime import datetime as dt
 import Sugestao
 import Unificar_XML
 import numpy as np
 import pandas
 import xml.etree.ElementTree as ElementTree
 import json
 import warnings
 import datetime
 from unidecode import unidecode
 import xlsxwriter
 import pytz
 import PySimpleGUI as psg
-from datetime import datetime as dt
 
-contador = 0
 
+contador = 0
 
 # Função recebe o resultado do cálculo entre vagas - matriculados e gera um análise
 def analisar_diferenca(diferenca):
     if diferenca > 0:
         return "Vagas Disponíveis"
     elif diferenca == 0:
         return "Não há vagas"
     elif diferenca < 0:
         return "Vagas excedidas"
     else:
         return ""
 
-
 # Função recebe matriculados,  diferença entre matriculados - capacidade para gerar uma análise das capacidades
 def analisar_capacidade(matriculados, diferenca, capacidade, sala):
     if diferenca > 0:
         return "Capacidade disponível"
     elif sala == "Sem sala":
         return "Sem sala"
     elif matriculados > 0 and diferenca == 0:
@@ -51,15 +48,14 @@
     elif capacidade == 0:
         return "Sem Capacidade"
     elif diferenca < 0:
         return "Capacidade excedida"
     else:
         return ""
 
-
 # Função recebe o XML Unificado e dois dicionários um de escolas e outro de turmas fictícias
 def armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f):
     tree_xml = ElementTree.parse(file_name_asc_xml)
     root = tree_xml.getroot()
     erro_log_turma = ""
     erro_log_sala = ""
 
@@ -160,54 +156,54 @@
         name = classrooms.get('name')
         short = classrooms.get('short')
 
         dict_classrooms[id] = name, short
 
     # armazenar a id como key e o name,short como value
     dict_class = {}
-    dict_multicom = {'2304': 'CURIE-M',
-                     '2236': 'ELIANE BRUM-M', '2237': 'ELIANE BRUM-N',
-                     '2225': 'MARCELLO SERPA-M',
-                     '2232': 'MARCELLO SERPA-N',
-                     '2238': 'MARGARIDA KUNSCH-M',
-                     '2214': 'PIAGET-N',
-                     '1031183': 'MARGARIDA KUNSCH-N',
-                     '2301': 'LISPECTOR-M',
-                     '2201': 'MONTESSORI-M',
-                     '2349': 'CLFS-N',
-                     '2249': 'FERMAT-N'}
+    dict_multicom = {
+    '2304': 'CURIE-M',
+    '2236': 'ELIANE BRUM-M', '2237': 'ELIANE BRUM-N',
+    '2225': 'MARCELLO SERPA-M',
+    '2232': 'MARCELLO SERPA-N',
+    '2238': 'MARGARIDA KUNSCH-M',
+    '2214': 'PIAGET-N',
+    '1031183':'MARGARIDA KUNSCH-N'
+    }
     for classes in root.iter("class"):
         # parametros
         id = classes.get('id')
         name = classes.get('name')
         short = classes.get('short')
+
         turmas_fic = dict(file_json_turmasfic)
-        if name.__contains__('Engenharia;') or name.__contains__('Multicom') or name.__contains__('Humanidades'):
+
+        if name.__contains__('Engenharia;') or name.__contains__('Multicom'):
             cr_curso = short.split(";")[5]
             periodo = short.split(";")[2]
             tipo = short.split(";")[3]
             turno = short.split(";")[4]
 
             chave_turma_fic = f"{cr_curso}|{periodo}"
 
             if cr_curso in dict_multicom.keys():
                 valor = dict_multicom[cr_curso]
                 new_name = f"{valor.split('-')[0]};{periodo};{tipo};{valor.split('-')[1]}"
 
                 name = new_name
 
             elif chave_turma_fic in turmas_fic.keys():
-                name = turmas_fic[chave_turma_fic]
+                    name = turmas_fic[chave_turma_fic]
 
-                new_name = f"{name};{periodo};{tipo};{turno}"
-                name = new_name
+                    new_name = f"{name};{periodo};{tipo};{turno}"
+                    name = new_name
             else:
-                contador += 1
-                f.write(f'#{contador} Aviso[Info]: erro ao converter a multicom name ={name} , short={short}''\n')
-                continue
+                    contador += 1
+                    f.write(f'#{contador} Aviso[Info]: erro ao converter a multicom name ={name} , short={short}''\n')
+                    continue
 
         dict_class[id] = name, short
 
     # armazenar a id como key e o period,days como value
     # para puxar a id da lesson e saber qual o horario e dia daquela aula
     dict_cards = {}
     for cards in root.iter("card"):
@@ -240,29 +236,27 @@
         id = lessons.get('id')
         subjectid = lessons.get('subjectid')
         groupid = lessons.get('groupids')
         classid = lessons.get('classids')
         classroomsid = lessons.get('classroomids')
 
         name_subject = dict_subject[subjectid]
-
         cr_curso = name_subject.split(';')[0]
 
         quantidade_turma = classid.count(',')
 
         posicao_turma = 0
 
         if quantidade_turma == 0:
             quantidade_turma = 1
         else:
             quantidade_turma += 1
 
         for i in range(0, quantidade_turma):
             try:
-
                 turma = str(dict_class[classid.split(',')[posicao_turma]]).replace(',', '/')
             except:
                 contador += 1
                 erro_log_turma += f'#{contador} Aviso[Ação]; Turma nao identificada na aula: {id}\n'
                 continue
 
             try:
@@ -333,15 +327,14 @@
 
             posicao_turma += 1
 
     f.write(erro_log_turma)
     f.write('\n\n')
     return valores
 
-
 # Função recebe o excel de capacidade e retorna apenas a abrev da sala e a sua capacidade
 def armazenaDadosCapacidade(file_name_capacidade, contador, f):
     # armazena os valores das colunas importantes
     todos_valores = []
 
     df = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2)
 
@@ -353,15 +346,14 @@
 
         posicao += 1
 
         todos_valores.append(f"{abrev_sala}|{capacidade}")
 
     return todos_valores
 
-
 def armazenaDadosTurmaDisciplina(file_name_turma_disciplina, file_json_sigla, contador, f):
     siglas = dict(file_json_sigla)
 
     def converteSigla(turma):
         if turma in siglas.keys():
             return siglas[turma]
         else:
@@ -425,22 +417,24 @@
         valores = f"{cr_curso}|{nome_curso}|{periodo}|{nome_turma}|{nome_disciplina}|{id_disciplina}|{divisao}|{dia}|{hora_inicio}|{hora_final}|" \
                   f"{agrupamento}|{turno}|{qtd_alunos}|{qtd_vagas}|{professor}|{estabelecimento}"
 
         todos_valores.append(valores)
 
     return todos_valores
 
-
 def gerarRelatorio(file_name_turma_disciplina, file_name_asc_xml, file_json_sigla, file_name_capacidade,
                    file_json_turmasfic, contador, file_json_escolas, file_json_tipos, f, file_name):
+
+    #transforma json em dict
     siglas = dict(file_json_sigla)
     escolas = dict(file_json_escolas)
     tipos = dict(file_json_tipos)
     log_sala = {}
 
+    #filter aviso
     warnings.simplefilter(action='ignore', category=UserWarning)
 
     def gerarTipo(tipo):
         if tipo in tipos.keys():
             return tipos[tipo]
         else:
             return tipo
@@ -460,57 +454,60 @@
     # armazenando dados
     array_turmas_disciplinas = armazenaDadosTurmaDisciplina(file_name_turma_disciplina, file_json_sigla, contador, f)
 
     array_asc_xml = armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f)
 
     array_capacidade = armazenaDadosCapacidade(file_name_capacidade, contador, f)
 
+    #dict que retorna capacidade
     dict_capacidade = {}
-
     for i in array_capacidade:
         abrev_sala = i.split('|')[0]
         capacidade = i.split('|')[1]
 
         dict_capacidade[abrev_sala] = str(capacidade)
 
+    today = dt.today()
+    if today.month > 6:
+        periodo = 2
+    else:
+        periodo = 1
+    ano_semestre = f'{today.year}/{periodo}'
+    # cria dict dos dados do Excel
     dict_valores = {}
     dict_retorna_cr_disciplina = {}
     retorna_horario_inicio = {}
     horario_repetido = []
     for i in array_turmas_disciplinas:
         # valores chave
         cr_curso_aluno = i.split('|')[0]
         periodo = i.split('|')[2]
-        nome_turma_final = i.split('|')[3].replace('- 2022/1', '').replace('2022/2', '').replace('2023/1', '').replace(
-            '2023/2', '')
-        nome_turma = i.split('|')[3].replace('- 2022/1', '').replace('-', '').replace('2022/2', '').replace('2023/1',
-                                                                                                            '').replace(
-            '2023/2', '')
+        nome_turma_final = i.split('|')[3].replace(f'{ano_semestre}', '')
+        nome_turma = i.split('|')[3].replace(f'- {ano_semestre}', '').replace('-', '')
         # valores
         nome_disciplina = i.split('|')[4]
         id_disciplina = i.split('|')[5]
         divisao = i.split('|')[6]
         dia = i.split('|')[7]
         escola = geraEscola(cr_curso_aluno)
         hora_final = i.split('|')[9]
         cr_disciplina = i.split('|')[5]
         nome_curso = i.split('|')[1]
         agrupamento = i.split('|')[10]
         turno = i.split('|')[11]
         qtd_alunos = i.split('|')[12]
         qtd_vagas = i.split('|')[13]
-        hora_inicio_old = f"{i.split('|')[8]}:".ljust(8, '0')[0:8] if i.split('|')[8] != '--' and i.split('|')[
-            8] != 'nan' else i.split('|')[8]
+        hora_inicio_old = f"{i.split('|')[8]}:".ljust(8, '0')[0:8] if i.split('|')[8] != '--' and i.split('|')[8] != 'nan' else i.split('|')[8]
         professor = i.split('|')[14]
         estabelecimento = i.split('|')[15]
         hora_inicio = str(hora_inicio_old.split(':')[:-1]).replace(',', ':').replace("'", "").replace("[", "").replace(
             "]", "").replace(' ', '')
         chave_dia = f"{periodo},{nome_turma},{cr_disciplina},{hora_inicio}".replace(' ', '').replace('2022/2',
                                                                                                      '').replace(
-            '2023/1', '').upper()
+            f'{ano_semestre}', '').upper()
         chave = f"{periodo},{nome_turma},{cr_disciplina},{hora_inicio},{dia},{divisao}".replace(' ', '').upper()
         tipo = gerarTipo(agrupamento)
 
         dict_valores[chave] = {
             'escola': escola,
             'cr_curso': cr_curso_aluno,
             'nome_disciplina': nome_disciplina,
@@ -527,14 +524,15 @@
             'qtd_alunos': qtd_alunos,
             'qtd_vagas': qtd_vagas,
             'professor': professor,
             'Tipo': tipo,
             'estabelecimento': estabelecimento
         }
 
+        # se a aula tiver mais de um horario salva todos na mesma chave
         chave_horario_repetido = f"{chave}{hora_inicio}"
         try:
             if chave_horario_repetido not in horario_repetido:
                 retorna_horario_inicio[chave_dia] += f"|{hora_inicio},{dia},{divisao}"
                 horario_repetido.append(chave_horario_repetido)
         except:
             retorna_horario_inicio[chave_dia] = f"{hora_inicio},{dia},{divisao}"
@@ -611,14 +609,16 @@
         try:
             if not dict_retorna_abrev_salaxml[sala].__contains__(abrev_sala):
                 dict_retorna_abrev_salaxml[sala] += f",{abrev_sala}"
                 # dict_retorna_abrev_salaxml[sala] = abrev_sala
         except:
             dict_retorna_abrev_salaxml[sala] = abrev_sala
 
+
+    #mescla os dados
     log_sem_salas = {}
     log_sala_abrev = {}
     log_sem_turmas_disciplinas = {}
     for dados in array_asc_xml:
         erro_repetido = []
         # barra invertida para poder retirar ela do texto
         barra = r"'\'"
@@ -635,16 +635,15 @@
         try:
             nome_disciplina = dados.split('|')[6].split(';')[2]
         except:
             f.write(dados.split('|')[6] + 'esta no formato errado')
             continue
 
         # - tratamento nome turma
-        turma = dados.split('|')[2].split('/')[0].replace(barra, '').replace(barra, '').replace(barra, '').replace(
-            barra, '').replace("'", '')
+        turma = dados.split('|')[2].split('/')[0].replace(barra, '').replace(barra, '').replace(barra, '').replace(barra, '').replace("'", '')
         turma = turma[1:]
         turma_nome = converteSigla(turma.split(';')[0])
         # turma utilizada para melhor entendimento
         turma_final = f"{turma_nome} - {periodo} - {abrev_turma.split(';')[3]} - {abrev_turma.split(';')[4]}"
         # turma utilizada como key
         nome_turma = f"{turma_nome}{periodo}{abrev_turma.split(';')[3]}{turma.split(';')[-1][0]}"
         try:
@@ -760,24 +759,29 @@
                 try:
                     valores = dict_valores[chave_dia_hora]
                 except:
                     contador += 1
                     f.write(f'#{contador} Aviso[Ação]: dia e hora nao encontrado ' + chave_dia_hora + '\n')
                     continue
                 # gerando dict que vai ser inserido no excel
-
+                today = dt.today()
+                if today.month > 6:
+                    periodo = 2
+                else:
+                    periodo = 1
+                ano_semestre = f'{today.year}/{periodo}'
                 dict_relatorio_final[key_final] = {
                     'Estabelecimento': valores['estabelecimento'],
                     'Escola': valores['escola'],
                     'CR Curso': str(valores['cr_curso'].split('.')[0]),
                     'Curso': valores['Curso'],
                     'Periodo': periodo,
                     'Sigla': valores['Agrupamento'],
                     'Tipo': valores['Tipo'],
-                    'Turma Prime': f"{valores['Nome_Turma']}2023/1",
+                    'Turma Prime': f"{valores['Nome_Turma']}{ano_semestre}",
                     'Nome disciplina': valores['nome_disciplina'],
                     'Turno': valores['Turno'],
                     'Divisão': valores['divisao'],
                     'Id disciplina': cr_disciplina,
                     'Qtde de Alunos Matri.': verifica_numero(valores['qtd_alunos']),
                     'Nr Vagas Cadastradas': verifica_numero(valores['qtd_vagas']),
                     'Dia': dia,
@@ -822,15 +826,15 @@
         if dados[1]['Divisão'] == ' ' or dados[1]['Divisão'] == '  ' or dados[1]['Divisão'] == '   ':
             dados[1]['Divisão'] = '-'
         if dados[1] not in valores_repetidos:
             Relatorio[dados[0]] = dados[1]
             valores_repetidos.append(dados[1])
 
     df = pandas.DataFrame(data=Relatorio)
-    df = (df.T)
+    df = df.T
     df = df.drop_duplicates()
 
     df.insert(14, 'Análise Vagas', '')
     df.insert(15, 'Diferença Vagas', '')
     df.insert(23, 'Análise Capacidade', '')
     df.insert(24, 'Diferença Capacidade', '')
 
@@ -1092,16 +1096,15 @@
     worksheet.set_column('R:R', 20)
     worksheet.set_column('S:S', 20)
     worksheet.set_column('T:T', 45)
     worksheet.set_column('U:U', 42)
     worksheet.set_column('V:V', 20)
     worksheet.set_column('W:W', 42)
 
-    df_capacidade = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2,
-                                      usecols=range(5, 26))
+    df_capacidade = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2,usecols=range(5, 26))
 
     df_capacidade.to_excel(writer, index=False, sheet_name="Ambientes de Aprendizagem")
 
     df_horarios = pandas.DataFrame()
 
     df_horarios["NOME ESPAÇO ASC"] = df_capacidade["NOME ESPAÇO ASC"]
 
@@ -1140,15 +1143,14 @@
     worksheet.set_column('A:A', 25)
     worksheet.set_column('B:B', 25)
     worksheet.set_column('C:C', 15)
 
     writer.close()
     return nome_arquivo
 
-
 def retorna_analista(escola):
     if escola == 'Belas Artes':
         analista = 'Diego'
 
     elif escola == 'Ciências da Vida':
         analista = 'Sheyla'
 
@@ -1167,54 +1169,52 @@
     elif escola == 'Politécnica':
         analista = 'Edivane'
     else:
         analista = 'não encontrado'
 
     return analista
 
-
 def verifica_numero(valor):
     try:
         numero = int(valor)
     except:
         if valor == "nan":
             numero = 0
         else:
             numero = float(valor)
             numero = int(numero)
     return numero
 
-
 def retorna_status(sala, diferenca, capacidade):
     if sala == 'Sem sala':
         valor = 'Sem sala'
     elif capacidade == '0' or capacidade == 0:
         valor = 'Sem info capacidade'
     elif diferenca < 0:
         valor = 'Lotada - rever ensalamento'
     elif diferenca < 5:
         valor = 'Próximo da capacidade'
     else:
         valor = 'Ok'
     return valor
 
-
-def main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name, caminho_auxiliar):
+def geracao_analise(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name,caminho_auxiliar):
     # pega somente o nome do arquivo para que o log seja salvo na mesma pasta
     utc_now = pytz.utc.localize(datetime.datetime.utcnow())
     dt_now = utc_now.astimezone(pytz.timezone("America/Sao_Paulo"))
     f = open(f"{caminho_auxiliar}/Log/{str(dt_now.strftime('%y-%m-%d %H-%M'))}.txt", "w+", encoding="utf8")
 
     file_name_turma_disciplina = arquivo_carga_horaria
 
     file_name_asc_xml = arquivo_xml
 
     file_name_capacidade = arquivo_capacidade
     print('Carregando...')
 
+    #salva arquivos auxiliares
     with open(f'{caminho_auxiliar}/siglas.json', 'r', encoding="utf-8") as j:
         file_json_sigla = json.loads(j.read())
 
     with open(f'{caminho_auxiliar}/turmasfic.json', 'r', encoding="utf-8") as j:
         file_json_turmasfic = json.loads(j.read())
 
     with open(f'{caminho_auxiliar}/escolas.json', 'r', encoding="utf-8") as j:
@@ -1223,24 +1223,21 @@
     with open(f'{caminho_auxiliar}/tipos.json', 'r', encoding="utf-8") as j:
         file_json_tipos = json.loads(j.read())
 
     nome_arquivo = gerarRelatorio(file_name_turma_disciplina, file_name_asc_xml, file_json_sigla, file_name_capacidade,
                                   file_json_turmasfic, contador, file_json_escolas, file_json_tipos, f, file_name)
     return nome_arquivo
 
-
-def gerarExcel(file_carga_horaria, file_capacidade, file_xml, file_name, caminho_aux):
+def gerarExcel(file_carga_horaria, file_capacidade, file_xml, file_name,caminho_aux):
     # le os valores vindo da tela
     arquivo_carga_horaria = file_carga_horaria
     arquivo_capacidade = file_capacidade
 
-    arquivo_xml = Unificar_XML.main(file_xml, caminho_aux)
+    arquivo_xml = Unificar_XML.main(file_xml,caminho_aux)
 
-    nome_arquivo = main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name, caminho_aux)
-
-    Sugestao.main(nome_arquivo, arquivo_capacidade, caminho_aux)
+    nome_arquivo = geracao_analise(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name,caminho_aux)
 
+    Sugestao.main(nome_arquivo, arquivo_capacidade,caminho_aux)
 
 if __name__ == '__main__':
-
-
     gerarExcel()
+
```

### Comparing `Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/PKG-INFO` & `Relatorio_Ensalamento-2.4.7/Relatorio_Ensalamento.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio-Ensalamento
-Version: 2.4.6
+Version: 2.4.7
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.6/Sugestao/Sugestao.py` & `Relatorio_Ensalamento-2.4.7/Sugestao/Sugestao.py`

 * *Files identical despite different names*

### Comparing `Relatorio_Ensalamento-2.4.6/Unificar_XML/Unificar_XML.py` & `Relatorio_Ensalamento-2.4.7/Unificar_XML/Unificar_XML.py`

 * *Files identical despite different names*

