# PPS-Unidad3Actividad2-JulioM

En esta segunda práctica de la unidad 3 tenemos como objetivos:

> Aprender y conocer comandos y herramientas para escanear y localizar equipos y recursos.
>
> Practicar y probar en el entorno de pruebas con dichas herramientas.
---
## ACTIVIDADES A REALIZAR
- Busca información de:
	- Como podemos obtener información pública con protocolo whois, web DoaminTools y DSNrecon.

        - WHOIS: Es un protocolo que permite consultar bases de datos para obtener información sobre la propiedad y el estado de un nombre de dominio en Internet. Al realizar una consulta WHOIS, se pueden obtener datos como el nombre del registrante, la fecha de registro y expiración del dominio, y los servidores de nombres asociados. 

        - DomainTools: Es una plataforma en línea que ofrece servicios avanzados de búsqueda WHOIS, proporcionando detalles sobre la propiedad de dominios, historial de direcciones IP, y más. Para utilizar DomainTools, se ingresa el nombre de dominio en su sitio web y se accede a la información recopilada. 

        - DNSRecon: Es una herramienta de código abierto diseñada para la enumeración de registros DNS de un dominio específico. Permite descubrir subdominios, registros MX, NS, y otros, facilitando la identificación de la infraestructura de red asociada a un dominio.

	- Cómo podemos utilizar Nmap y nikto,   para buscar equipos, puertos abiertos, servicios, vulnerabilidades.

        - Nmap: Es una herramienta de escaneo de redes que permite detectar hosts activos, puertos abiertos y servicios en ejecución. Además, mediante el uso de scripts NSE (Nmap Scripting Engine), Nmap puede identificar vulnerabilidades específicas en los servicios detectados. Por ejemplo, el script vuln permite detectar vulnerabilidades conocidas en los sistemas analizados. 

        - Nikto: Es un escáner de servidores web que detecta vulnerabilidades en aplicaciones web, como configuraciones inseguras, archivos y programas potencialmente peligrosos, y versiones desactualizadas de software. Nikto realiza pruebas exhaustivas en servidores web para identificar posibles puntos débiles.

	- Cómo utilizar Wfuzz, Dirb para localizar recursos web en servidores.

        - Wfuzz: Es una herramienta diseñada para realizar pruebas de fuerza bruta en aplicaciones web, permitiendo descubrir recursos ocultos como archivos y directorios no listados. Mediante el uso de diccionarios personalizados, Wfuzz envía solicitudes HTTP para identificar estos recursos.

        - Dirb: Funciona de manera similar a Wfuzz, enfocándose en la enumeración de directorios y archivos en servidores web. Utiliza listas predefinidas de nombres comunes para detectar recursos que no están directamente accesibles o indexados.

	- Que scripts que podemos utilizar con Nmap para la búsqueda de vulnerabilidades.

        - vuln: Detecta vulnerabilidades conocidas en los servicios identificados durante el escaneo.

        - http-vuln-cve2017-5638: Verifica si un servidor es vulnerable a la vulnerabilidad CVE-2017-5638 en Apache Struts.

        - ssl-heartbleed: Comprueba si un servidor es vulnerable a la vulnerabilidad Heartbleed en OpenSSL.

Un ejemplo de como utilizarlo es con el comando:

            **nmap --script vuln 192.168.1.1**

	- Cómo podemos buscar información de explotación de vulnerabilidades con searchsploit

        - SearchSploit: Es una herramienta que permite buscar y acceder a exploits disponibles en la base de datos de Exploit-DB desde la línea de comandos. Es especialmente útil para identificar exploits relacionados con vulnerabilidades detectadas en sistemas o aplicaciones.

Un ejemplo de búsqueda es con el comando:

            **searchsploit vsftpd 2.3.4**


- Instala en tu navegador la extensión de Shodan y muestra la información que tenemos tanto de ip, como de dominio del sitio http://iesvalledeljerteplasencia.es 
- Sobre la red del laboratorio PPS con kali, bWAPP, Multidillae y DVWA:<
	- Ayudándote del fichero docker-compose localiza las diferentes máquinas y puertos que deberían de tener abiertos.
	- Identifica los equipos de la Red con Nmap.
	- Realiza análisis de puertos en las MV.
	- Encuentra los Servicios y Sistemas Operativos de las MV.
	- Inspecciona los puertos con nikto.
	- Busca las vulnerabilidades de las MV con los scripts de Nmap.
	- Localiza los servicios web que tienen las diferentes máquinas (Wfuzz y Dirb).
	- Utiliza el comando searchsploit para buscar información de explotación de vulnerabilidades presentes en linux con kernel 5
---	
## ENTREGA

>__Realiza las operaciones indicadas__

>__Crea un repositorio  con nombre PPS-Unidad3Actividad2-Tu-Nombre donde documentes la realización de ellos.__

> No te olvides de documentarlo convenientemente con explicaciones, capturas de pantalla, etc.

>__Sube a la plataforma, tanto el repositorio comprimido como la dirección https a tu repositorio de Github.__