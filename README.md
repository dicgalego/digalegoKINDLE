# Dicionario da lingua galega (RAG)

O dicionario é o da RAG, sen exemplos.

1.- Ficheiro MOBI.
  É a versión para o firmware orixinal do Kindle.
  Utilización: copiar o ficheiro ao cartafol "documents" do Kindle.
  Importante: 
    Non conseguín que co último firmware actualizado (5.6.1.1, para o PW1) abrise por defecto o dicionario da RAG para libros cos metadatos correctos (lang:glg ou gl): abre o dicionario de portugués. Como nos últimos firmwares permite escoller o dicionario, é un problema menor.
    
2.- Formato STARDICT.
  Son os ficheiros galician.dict, galician.idx e galician.ifo.
  Eu utilízoos co firmware alternativo para Kindle "Duokan".
  Poderíase utilizar con calquera lector electrónico ou aplicativo que admita o formato stardict ou pódense empregar para convertilos noutro formato de dicionario.
  
 # Cómo se fixo?
 
 - Partíase do dicionario RAG nunha base de datos sqlite3. Os datos estaban todos nunha táboa.
 - Fíxose un dump da táboa que interesaba e obtívose un ficheiro CSV coas diferentes entradas en código HTML.
 - Coas ferramentas tr, sed, awk, e pup obtívose un ficheiro TSV (lema TAB definición(s)).
 - Con penelope creáronse os dicionarios en MOBI e STARDICT.
 
