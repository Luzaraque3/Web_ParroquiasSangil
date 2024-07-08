# Web_ParroquiasSangil
Sitio web de las Parroquias de San Gil

Javascrip "
// Datos simulados de las parroquias
const parroquias = [
    { nombre: "Catedral Metropolitana de San Gil", direccion: "Calle 12 #8-32" },
    { nombre: "Basílica Menor de la Santa Cruz", direccion: "Parque Principal" },
    { nombre: "Iglesia de San Agustín", direccion: "Carrera 9 #10-15" },
    { nombre: "Capilla de la Virgen de Chiquinquirá", direccion: "Barrio Libertadores" }
];

// Función para mostrar las parroquias en la página
function mostrarParroquias() {
    const parroquiasContainer = document.getElementById('parroquias');
    parroquias.forEach(parroquia => {
        const parroquiaDiv = document.createElement('div');
        parroquiaDiv.classList.add('parroquia');
        parroquiaDiv.innerHTML = `
            <h3>${parroquia.nombre}</h3>
            <p><strong>Dirección:</strong> ${parroquia.direccion}</p>
        `;
        parroquiasContainer.appendChild(parroquiaDiv);
    });
}

// Llama a la función al cargar la página
window.onload = mostrarParroquias;

"
