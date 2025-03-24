<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hoja de Vida CV - Mayerli Alejandra Castillo Yandun</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Times New Roman', sans-serif;
        }
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: #e0f7fa; /* Color de fondo azul agua suave */
            color: #333;
        }
        .container {
            display: flex;
            flex-direction: row;
            width: 100%;
            max-width: 1300px;
            height: auto;
            background: white; /* Fondo blanco para el contenedor */
            color: #004d40;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
        }
        .sidebar {
            width: 30%;
            background: #00796b; /* Color verde agua para la barra lateral */
            color: white;
            text-align: center;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .sidebar img {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 3px solid white; /* Borde blanco */
            margin-bottom: 15px;
        }
        .contact-info {
            background: #00796b; /* Color verde agua para la sección de contacto */
            color: white;
            padding: 10px;
            border-radius: 5px;
            width: 100%; /* Asegura que ocupe todo el ancho */
            margin-top: 10px; /* Espaciado superior */
        }
        .contact-info a {
            color: #000; /* Color negro para el texto del correo y teléfono */
        }
        .main-content {
            width: 70%;
            padding: 20px;
            overflow-y: auto;
            background: #e0f7fa; /* Color de fondo azul agua suave */
        }
        .title {
            font-size: 26px;
            font-weight: bold;
            text-align: center;
            margin-bottom: 20px;
            color: #00796b; /* Color verde agua para el título */
        }
        .bio, .portfolio {
            margin-bottom: 20px;
        }
        .bio h2, .portfolio h2 {
            color: #004d40; /* Color verde oscuro para encabezados */
            border-bottom: 2px solid #00796b; /* Color verde agua para el borde */
            padding-bottom: 5px;
            margin-bottom: 10px;
        }
        .bio p {
            font-size: 14px;
            color: #333; /* Color del texto de la biografía */
            text-align: justify; /* Justificar el texto de la biografía */
        }
        .interests {
            margin-bottom: 20px;
        }
        .interests h2 {
            margin-bottom: 10px;
        }
        .interests ul {
            list-style: none;
            padding-left: 0;
            display: flex;
            flex-direction: column; /* Alinear verticalmente */
            align-items: flex-start; /* Alinear a la izquierda */
        }
        .interests li {
            font-size: 14px;
            color: #333; /* Color del texto de los intereses */
            margin-bottom: 5px; /* Espaciado entre los elementos de la lista */
            display: flex; /* Usar flexbox para alinear icono y texto */
            align-items: center; /* Centrar verticalmente el icono y el texto */
        }
        .interests li i {
            margin-right: 8px; /* Espaciado entre el icono y el texto */
        }
        .portfolio .tabs {
            display: flex;
            justify-content: space-between; /* Espacio entre los botones */
            background: #00796b; /* Color verde agua para las pestañas */
            color: white;
            padding: 8
            border-radius: 5px;
            flex-wrap: nowrap; /* Asegura que los botones estén en una sola fila */
            overflow-x: auto; /* Permite desplazamiento horizontal si es necesario */
        }
        .portfolio .tabs div {
            flex: 0 0 auto; /* Evita que los botones se ajusten y permite que mantengan su tamaño */
            text-align: center;
            padding: 7px;
            cursor: pointer;
            transition: background 0.3s, color 0.3s;
            margin: 5px; / 
        }
        .portfolio .tabs div:hover {
            background: #555355;
        }
        .portfolio .tabs div.active {
            background: #555355;
            font-weight: bold;
        }
        .tab-content {
            display: none;
            padding: 8px;
            background: #ecf0f1;
            border-radius: 4px;
            margin-top: 8px;
            color: #13012f;
        }
        .tab-content.active {
            display: block;
        }
        .year {
            background: #00796b;
            padding: 8px;
            margin: 4px 0;
            border-radius: 4px;
            cursor: pointer;
            font-weight: bold;
            text-align: center;
            transition: background 0.3s;
        }
        .year:hover {
            background: #555355;
        }
        .year-content {
            display: none;
            padding: 4px 8px;
            background: white;
            border-left: 3px solid #27292b;
            margin-top: 4px;
        }
        /* Estilos para los enlaces externos */
        .links {
            display: flex;
            flex-direction: column; /* Asegura que los enlaces estén uno debajo del otro */
            align-items: center; /* Centra los enlaces */
            margin-top: 20px;
        }
        .links a {
            color: white;
            text-decoration: none;
            margin: 5px 0; /* Espaciado entre enlaces */
            padding: 10px;
            border: 1px solid transparent; /* Para que el área de clic sea más grande */
            border-radius: 5px;
            transition: background 0.3s, color 0.3s;
            width: 100%; /* Asegura que los enlaces ocupen todo el ancho disponible */
            text-align: center; /* Centra el texto en los enlaces */
        }
        .links a:hover {
            background: #777474; /* Color de fondo al pasar el mouse */
            color: white; /* Color del texto al pasar el mouse */
        }
        /* Responsivo */
        @media (max-width: 768px) {
            .container {
                flex-direction: column;
            }
            .sidebar {
                width: 100%;
                padding: 20px;
            }
            .main-content {
                width: 100%;
                padding: 20px;
            }
            .sidebar img {
                width: 100px; /* Ajustar el tamaño de la imagen en móviles */
                height: 100px;
            }
            .bio p, .interests li {
                font-size: 12px; /* Ajustar el tamaño de la fuente en móviles */
            }
            .title {
                font-size: 22px; /* Ajustar el tamaño del título en móviles */
            }
            .portfolio .tabs {
                flex-direction: column; /* Cambiar a columna en móviles */
            }
            .portfolio .tabs div {
                padding: 10px; /* Aumentar el padding para mejor clicabilidad */
                margin: 5px 0; /* Espaciado entre botones */
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Barra lateral -->
        <div class="sidebar">
           <img src="https://raw.githubusercontent.com/Maye2002/CV/main/Imagen%20de%20WhatsApp%202025-03-22%20a%20las%2022.36.30_ee548773.jpg" alt="Foto de perfil">
            <h2>Mayerli Alejandra Castillo Yandun</h2>
            <div class="contact-info">
                <p><strong>Correo:</strong> <a href="mailto:mayecastillo762@gmail.com"><i class="fas fa-envelope"></i> mayecastillo762@gmail.com</a></p>
                <p><strong>Teléfono:</strong> <a href="tel:+593985288070"><i class="fas fa-phone"></i> +593 985288070</a></p>
            </div>
            <br>
            <div class="links">
                <h3>Links Externos</h3>
                <a href="https://upecedu-my.sharepoint.com/:b:/g/personal/mayerli_castillo_upec_edu_ec/EQhp6O81p3hIhUePyd_7XCwBIv_-5ndALea_1qMsGfQEHA?e=v1QWWk"><i class="fas fa-file-pdf" style="color: #FF6F61;"></i> Hoja de vida PDF</a>
                <a href="https://www.linkedin.com/in/mayerli-castillo-920437357/"><i class="fab fa-linkedin" style="color: #1E88E5;"></i> LinkedIn</a>
            </div>
        </div>
        <!-- Sección Principal -->
        <div class="main-content">
            <div class="title">Hoja de Vida CV</div>
            <div class="bio">
                <h2><i class="fas fa-user"></i> Biografía</h2>
                <p> Nací en Tulcán, Ecuador, en el año 2002. Cuento con título de tercer nivel de ingeniería en Logística
                    y Transporte en la Universidad Politécnica Estatal del Carchi.
                    He desarrollado habilidades en herramientas tecnológicas con conocimientos en logística, gestión de
                    almacenes, inventarios, análisis de datos manejado de indicadores clave (KPIs), lo que me permite analizar
                    y mejorar procesos en el ámbito del transporte y la gestión operativa. Intereses profesionales: gestión en
                    cadena de suministros, optimización de rutas de transporte, gestión de inventarios y almacenamiento.
                    Habilidad para trabajar en equipo, aprender con facilidad y resolver problemas de manera eficiente.
                    Disponibilidad inmediata y flexibilidad para horarios y ubicación.</p>
            </div>
            <div class="interests">
                <h2><i class="fas fa-briefcase"></i> Intereses Profesionales</h2>
                <ul>
                    <li><i class="fas fa-truck"></i> Logística y Transporte – Gestión de la cadena de suministro</li>
                    <li><i class="fas fa-industry"></i> Logística y Transporte – Optimización de procesos productivos</li>
                    <li><i class="fas fa-map-marked-alt"></i> Logística y Transporte – Gestión de rutas de transporte</li>
                    <li><i class="fas fa-file-invoice"></i> Comercio exterior – Gestión de documentación aduanera</li>
                    <li><i class="fas fa-globe"></i> Comercio exterior – Normativas internacionales de comercio</li>
                </ul>
            </div>
            <div class="portfolio">
                <h2><i class="fas fa-folder-open"></i> Portafolio de Proyectos</h2>
                <div class="tabs">
                    <div class="tab-btn" onclick="showTab('consultoria', this)"><i class="fas fa-graduation-cap"></i> Formación Académica</div>
                    <div class="tab-btn" onclick="showTab('investigacion', this)"><i class="fas fa-flask"></i> Proyectos Investigación</div>
                    <div class="tab-btn" onclick="showTab('cursos', this)"><i class="fas fa-book"></i> Cursos</div>
                    <div class="tab-btn" onclick="showTab('colaboraciones', this)"><i class="fas fa-handshake"></i> Colaboraciones</div>
                    <div class="tab-btn" onclick="showTab('idiomas', this)"><i class="fas fa-language"></i> Idiomas</div> 
                    <div class="tab-btn" onclick="showTab('software', this)"><i class="fas fa-laptop-code"></i> Experiencia</div>
                    <div class="tab-btn" onclick="showTab('premios', this)"><i class="fas fa-trophy"></i> Distinciones, Premios o Becas</div>
                    <div class="tab-btn" onclick="showTab('contenido', this)"><i class="fas fa-file-alt"></i> Desarrollo de Contenido Virtual y Prototipos</div>
                </div>
                <!-- Proyectos consultoría -->
                <div id="consultoria" class="tab-content active">
                    <div class="year" onclick="toggleYear('pc2025')">2025</div>
                    <div id="pc2025" class="year-content">
                        <ul>
                            <li>Ingeniería en Logística y Transporte en la Universidad Politécnica Estatal Del Carchi</li>
                        </ul>
                    </div>
                </div>
                <!-- Proyectos Investigación -->
                <div id="investigacion" class="tab-content">
                    <div class="year" onclick="toggleYear('pi2025')">2025</div>
                    <div id="pi2025" class="year-content">
                        <ul>
                            <li>Factores de riesgo para el transporte y la eficiencia logística en la empresa de transporte Ameex isCargo S.A. Universidad Politécnica Estatal del Carchi.</li>
                        </ul>
                    </div>
                </div>
                <!-- Cursos -->
                <div id="cursos" class="tab-content">
                    <div class="year" onclick="toggleYear('c20251')">2025</div>
                    <div id="c20251" class="year-content">
                        <ul>
                            <li>Excel Intermedio. Duración: 20 horas. TEACHLR. Modalidad Virtual. 17-28 de marzo, 2025.</li>
                        </ul>
                    </div>
                    <div class="year" onclick="toggleYear('c2024')">2024</div>
                    <div id="c2024" class="year-content">
                        <ul>
                            <li>Práctica en el llenado de declaraciones Aduaneras en el Sistema Aduanero. Duración: 10 horas. My Intelecto. Guayaquil, Ecuador. 12-24 de noviembre, 2024.</li>
                            <li>Actividades Simultáneas Latinoamericanas de Estudiantes e Ingenieros Industriales. Duración: 6 horas. Universidad del Istmo. Modalidad Virtual Panamá. 10 de mayo, 2024.</li>
                        </ul>
                    </div>
                </div>
                <!-- Nueva sección de idiomas -->
                <div id="idiomas" class="tab-content">
                    <div class="year" onclick="toggleYear('nat2000')">Nativo</div>
                    <div id="nat2000" class="year-content">
                        <ul>
                            <li><strong>Español:</strong> Nativo</li>
                        </ul>
                    </div>
                    <div class="year" onclick="toggleYear('idiomas2025')">2025</div>
                    <div id="idiomas2025" class="year-content">
                        <ul>
                             <li><strong>Inglés:</strong> Nivel B1 – Certificado por la Universidad Politécnica Estatal del Carchi (2022)</li>
                        </ul>
                     </div>
                </div>
                <!-- Colaboraciones -->
                <div id="colaboraciones" class="tab-content">
                    <div class="year" onclick="toggleYear('col2024')">2024</div>
                    <div id="col2024" class="year-content">
                        <ul>
                            <li>Proyecto de Vinculación con la Sociedad denominado “Diseño de rutas para el mejoramiento del servicio de transporte comercial, modalidad escolar e institucional con las operadoras domiciliadas en la ciudad de Tulcán”.</li>
                        </ul>
                    </div>
                </div>
                <!-- Experiencia en Software -->
                <div id="software" class="tab-content">
                    <div class="year" onclick="toggleYear('sof12')">Experiencia en Software</div>
                    <div id="sof12" class="year-content">
                        <ul>
                            <li><i class="fab fa-microsoft"></i> Microsoft Excel (Intermedio) - Analizar base de datos con funciones avanzadas</li>
                            <li><i class="fas fa-chart-line"></i> Power Bi (Básico) - Presentación de informes y análisis de datos</li>
                            <li><i class="fas fa-drafting-compass"></i> Auto Cad (Básico) - Diseño y modelado de plantas de producción</li>
                            <li><i class="fas fa-cogs"></i> Flexsim (Básico) - Simulación de procesos productivos</li>
                            <li><i class="fas fa-map-marked-alt"></i> Arc Map (Básico) - Diseño y optimización de rutas</li>
                            <li><i class="fas fa-paint-brush"></i> Sketchup (Básico) - Creación de modelos personalizados</li>
                            <li><i class="fab fa-python"></i> Python (Básico) - Desarrollo de scripts para análisis de datos</li>
                        </ul>
                    </div>
                    <div class="year" onclick="toggleYear('expp')">Experiencia Profesional</div>
                    <div id="expp" class="year-content">
                        <ul>
                            <li>2023: Prácticas preprofesionales en Encomiendas Ecuador S.A recolección y distribución en paquetería, digitación de guías.</li>    
                        </ul>
                    </div>
                </div>
                <!-- Distinciones, Premios o Becas -->
                <div id="premios" class="tab-content">
                    <div class="year" onclick="toggleYear('pre11')">2025</div>
                    <div id="pre11" class="year-content">
                        <ul>
                            <li><i class="fas fa-trophy"></i> Beca Excelencia Académica</li>
                        </ul>
                    </div>
                    <div class="year" onclick="toggleYear('pre10')">2023</div>
                    <div id="pre10" class="year-content">
                        <ul>
                            <li><i class="fas fa-award"></i> Beca Socioeconómica</li>           
                        </ul>
                    </div>
                </div>
                <!-- Desarrollo de Contenido Virtual y Prototipos -->
                <div id="contenido" class="tab-content">
                    <ul>
                        <li><i class="fas fa-file-alt"></i> Diseño de rutas para el mejoramiento del servicio de transporte comercial, modalidad escolar e institucional con las operadoras domiciliadas en la ciudad de Tulcán con el software ARC MAP</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
    <script>
        function showTab(tabName, element) {
            document.querySelectorAll('.tab-content').forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabName).classList.add('active');
            document.querySelectorAll('.tab-btn').forEach(btn => btn.classList.remove('active'));
            element.classList.add('active');
        }
        function toggleYear(yearId) {
            let yearContent = document.getElementById(yearId);
            yearContent.style.display = yearContent.style.display === 'block' ? 'none' : 'block';
        }
    </script>
</body>
</html>
