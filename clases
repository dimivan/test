class Usuario {
    constructor(nombre, apellido, mascotas, libros) {
        this.nombre = nombre
        this.apellido = apellido
        this.libros = libros
        this.mascotas = mascotas
    }

    getFullNme(){
        return this.nombre + ' ' + this.apellido
    }

    addMascota(mascota) {
        if(!this.mascota || !Array.isArray(this.mascota) ){
            this.mascotas = []
        }
        this.mascotas.push(mascota)
    }

    countMascotas() {
        return (this.mascotas && Array.isArray(this.mascotas.length)) ? this.mascotas.length : 0
    }

    addLibro(nombre, autor) {
        if(!this.libros || !Array.isArray(this.libros) ){
            this.libros = []
        }
        this.libros.push({nombre: nombre, autor: autor })
    }

    getBookNames() {
        return (this.libros && Array.isArray(this.libros)) ? this.libros.map(element => {return element.nombre }) : []
    }
}

const usuario = new Usuario(
  'Axel',
  'Zapata',
  ['Pelusa', 'Pelos', 'Canelita'],
  [{nombre: '1984', autor:'George Orwell'}, {nombre: 'Un mundo feliz', autor: 'aldous huxley'}])

  // console.log(usuario)
  console.log('Libros: ' + usuario.getBookNames())
  usuario.addLibro('El señor de las moscas','William Golding')
  console.log('Libros: ' + usuario.getBookNames())
  console.log(usuario.getFullNme())
  console.log('Mascotas: ' + usuario.countMascotas())
  usuario.addMascota('Peludito')
  console.log('Mascotas: ' + usuario.countMascotas())
