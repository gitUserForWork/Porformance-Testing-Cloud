======================
FunkLoad_ bench report
======================


:date: 2013-11-11 03:02:58
:abstract: Stress Testing on user supplied link
           Bench result of ``Stress.test_stress``: 
           Access (nb_time)s times the main url

.. _FunkLoad: http://funkload.nuxeo.org/
.. sectnum::    :depth: 2
.. contents:: Table of contents
.. |APDEXT| replace:: \ :sub:`1.5`

Bench configuration
-------------------

* Launched: 2013-11-11 03:02:58
* From: mayank
* Test: ``test_Stress.py Stress.test_stress``
* Target server: https://facebook.com
* Cycles of concurrent users: [10, 50, 25]
* Cycle duration: 10s
* Sleeptime between request: from 0.0s to 0.5s
* Sleeptime between test case: 0.01s
* Startup delay between thread: 0.01s
* Apdex: |APDEXT|
* FunkLoad_ version: 1.16.1


Test stats
----------

The number of Successful **Tests** Per Second (STPS) over Concurrent Users (CUs).

Sorry no test have finished during a cycle, the cycle duration is too short.


Page stats
----------

The number of Successful **Pages** Per Second (SPPS) over Concurrent Users (CUs).
Note that an XML RPC call count like a page.

 .. image:: pages_spps.png
 .. image:: pages.png

 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                CUs             Apdex*             Rating               SPPS            maxSPPS              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                 10              1.000          Excellent              2.000             10.000                 20                 20             0.00%              1.115              4.776              8.708              1.123              7.938              8.698              8.708
                 50              0.999          Excellent             10.000             44.000                100                100             0.00%              1.104              4.948              9.434              1.112              7.706              9.327              9.388
                 25              1.000          Excellent              5.000             25.000                 50                 50             0.00%              1.104              4.844              9.103              1.110              7.956              8.960              8.972
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

 \* Apdex |APDEXT|

Request stats
-------------

The number of **Requests** Per Second (RPS) successful or not over Concurrent Users (CUs).

 .. image:: requests_rps.png
 .. image:: requests.png

 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                CUs             Apdex*            Rating*                RPS             maxRPS              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                 10              1.000          Excellent              9.900             11.000                 99                 99             0.00%              0.817              0.965              1.343              0.883              0.934              1.126              1.147
                 50              0.999          Excellent             53.800             57.000                538                538             0.00%              0.029              0.920              1.513              0.828              0.938              1.109              1.130
                 25              1.000          Excellent             25.200             29.000                252                252             0.00%              0.155              0.961              1.460              0.855              0.947              1.113              1.135
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

 \* Apdex |APDEXT|

Slowest requests
----------------

The 5 slowest average response time during the best cycle with **50** CUs:

* In page 001, Apdex rating: Excellent, avg response time: 1.12s, get: ````
  `Get url`
* In page 001, Apdex rating: Excellent, avg response time: 0.99s, link: ``/``
  ``
* In page 001, Apdex rating: Excellent, avg response time: 0.97s, link: ``/``
  ``
* In page 001, Apdex rating: Excellent, avg response time: 0.96s, link: ``/``
  ``
* In page 001, Apdex rating: Excellent, avg response time: 0.96s, get: ``/``
  ``

Page detail stats
-----------------


PAGE 001: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ````

     .. image:: request_001.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              1.115              1.130              1.147              1.123              1.128              1.147              1.147
                     50              1.000          Excellent                 50                 50             0.00%              1.104              1.124              1.152              1.108              1.125              1.142              1.145
                     25              1.000          Excellent                 25                 25             0.00%              1.104              1.124              1.149              1.108              1.123              1.148              1.149
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 002, get, url ``/``

     .. image:: request_001.002.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.918              0.975              1.056              0.931              0.949              1.056              1.056
                     50              1.000          Excellent                 50                 50             0.00%              0.837              0.958              1.103              0.885              0.950              1.044              1.064
                     25              1.000          Excellent                 25                 25             0.00%              0.852              0.969              1.057              0.913              0.955              1.047              1.057
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 003, link, url ``/``

     .. image:: request_001.003.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.898              0.960              1.158              0.905              0.935              1.158              1.158
                     50              1.000          Excellent                 50                 50             0.00%              0.795              0.916              1.061              0.857              0.910              0.989              1.005
                     25              1.000          Excellent                 25                 25             0.00%              0.778              0.930              1.057              0.850              0.932              1.014              1.023
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 004, link, url ``/``

     .. image:: request_001.004.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.887              0.922              0.958              0.892              0.920              0.958              0.958
                     50              0.990          Excellent                 50                 50             0.00%              0.813              0.963              1.513              0.898              0.956              1.035              1.040
                     25              1.000          Excellent                 25                 25             0.00%              0.865              0.957              1.112              0.894              0.947              1.059              1.074
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 005, link, url ``/``

     .. image:: request_001.005.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.842              0.909              1.003              0.869              0.902              1.003              1.003
                     50              1.000          Excellent                 50                 50             0.00%              0.773              0.915              1.133              0.818              0.917              1.014              1.057
                     25              1.000          Excellent                 25                 25             0.00%              0.764              0.918              1.065              0.835              0.920              1.038              1.041
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 006, link, url ``/``

     .. image:: request_001.006.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.873              0.935              1.107              0.885              0.923              1.107              1.107
                     50              1.000          Excellent                 50                 50             0.00%              0.777              0.942              1.152              0.849              0.934              1.040              1.046
                     25              1.000          Excellent                 25                 25             0.00%              0.821              0.982              1.460              0.858              0.930              1.089              1.408
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 007, link, url ``/``

     .. image:: request_001.007.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.892              0.951              1.148              0.913              0.939              1.148              1.148
                     50              1.000          Excellent                 50                 50             0.00%              0.813              0.968              1.292              0.898              0.956              1.057              1.095
                     25              1.000          Excellent                 25                 25             0.00%              0.880              0.950              1.023              0.889              0.959              0.988              1.005
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 008, link, url ``/``

     .. image:: request_001.008.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.817              0.921              1.094              0.837              0.912              1.094              1.094
                     50              1.000          Excellent                 50                 50             0.00%              0.775              0.929              1.401              0.829              0.923              1.019              1.043
                     25              1.000          Excellent                 25                 25             0.00%              0.779              0.953              1.190              0.800              0.939              1.046              1.138
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 009, link, url ``/``

     .. image:: request_001.009.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                 10                 10             0.00%              0.896              1.023              1.343              0.904              1.003              1.343              1.343
                     50              1.000          Excellent                 50                 50             0.00%              0.869              0.988              1.475              0.914              0.957              1.050              1.156
                     25              1.000          Excellent                 25                 25             0.00%              0.875              0.989              1.181              0.884              0.956              1.121              1.145
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 010, link, url ``/``

     .. image:: request_001.010.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                  9                  9             0.00%              0.882              0.916              0.942              0.882              0.920              0.942              0.942
                     50              1.000          Excellent                 47                 47             0.00%              0.761              0.930              1.396              0.825              0.928              1.018              1.042
                     25              1.000          Excellent                 22                 22             0.00%              0.825              0.911              1.020              0.828              0.907              1.006              1.008
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|

Definitions
-----------

* CUs: Concurrent users or number of concurrent threads executing tests.
* Request: a single GET/POST/redirect/xmlrpc request.
* Page: a request with redirects and resource links (image, css, js) for an html page.
* STPS: Successful tests per second.
* SPPS: Successful pages per second.
* RPS: Requests per second, successful or not.
* maxSPPS: Maximum SPPS during the cycle.
* maxRPS: Maximum RPS during the cycle.
* MIN: Minimum response time for a page or request.
* AVG: Average response time for a page or request.
* MAX: Maximmum response time for a page or request.
* P10: 10th percentile, response time where 10 percent of pages or requests are delivered.
* MED: Median or 50th percentile, response time where half of pages or requests are delivered.
* P90: 90th percentile, response time where 90 percent of pages or requests are delivered.
* P95: 95th percentile, response time where 95 percent of pages or requests are delivered.
* Apdex T: Application Performance Index, 
  this is a numerical measure of user satisfaction, it is based
  on three zones of application responsiveness:

  - Satisfied: The user is fully productive. This represents the
    time value (T seconds) below which users are not impeded by
    application response time.

  - Tolerating: The user notices performance lagging within
    responses greater than T, but continues the process.

  - Frustrated: Performance with a response time greater than 4*T
    seconds is unacceptable, and users may abandon the process.

    By default T is set to 1.5s this means that response time between 0
    and 1.5s the user is fully productive, between 1.5 and 6s the
    responsivness is tolerating and above 6s the user is frustrated.

    The Apdex score converts many measurements into one number on a
    uniform scale of 0-to-1 (0 = no users satisfied, 1 = all users
    satisfied).

    Visit http://www.apdex.org/ for more information.
* Rating: To ease interpretation the Apdex
  score is also represented as a rating:

  - U for UNACCEPTABLE represented in gray for a score between 0 and 0.5 

  - P for POOR represented in red for a score between 0.5 and 0.7

  - F for FAIR represented in yellow for a score between 0.7 and 0.85

  - G for Good represented in green for a score between 0.85 and 0.94

  - E for Excellent represented in blue for a score between 0.94 and 1.

Report generated with FunkLoad_ 1.16.1, more information available on the `FunkLoad site <http://funkload.nuxeo.org/#benching>`_.