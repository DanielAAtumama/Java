import java.util.ArrayList;
import java.util.Collections;

public class Main {
    public static void main(String[] args) {
        // 1. Declarar un ArrayList vacío
        ArrayList<Integer> arrayListVacio = new ArrayList<>();

        // 2. Declarar un ArrayList con más de 5 elementos
        ArrayList<Integer> arrayListMasDe5 = new ArrayList<>();
        arrayListMasDe5.add(1);
        arrayListMasDe5.add(2);
        arrayListMasDe5.add(3);
        arrayListMasDe5.add(4);
        arrayListMasDe5.add(5);
        arrayListMasDe5.add(6);

        // 3. Encuentra la longitud de los dos ArrayLists creados anteriormente.
        int longitudArrayListVacio = arrayListVacio.size();
        int longitudArrayListMasDe5 = arrayListMasDe5.size();

        System.out.println("Longitud del ArrayList vacío: " + longitudArrayListVacio);
        System.out.println("Longitud del ArrayList con más de 5 elementos: " + longitudArrayListMasDe5);

        // 4. Obtén el primer elemento, el elemento central y el último elemento del ArrayList.
        int primerElemento = arrayListMasDe5.get(0);
        int elementoCentral = arrayListMasDe5.get(arrayListMasDe5.size() / 2);
        int ultimoElemento = arrayListMasDe5.get(arrayListMasDe5.size() - 1);

        System.out.println("Primer elemento del ArrayList: " + primerElemento);
        System.out.println("Elemento central del ArrayList: " + elementoCentral);
        System.out.println("Último elemento del ArrayList: " + ultimoElemento);

        // 5. Crear un ArrayList llamado Datos_personales que contenga (nombre, edad, altura, estado civil, dirección), y agrega datos utilizando el método add().
        ArrayList<String> datosPersonales = new ArrayList<>();
        datosPersonales.add("Daniel");
        datosPersonales.add("19");
        datosPersonales.add("1.90m");
        datosPersonales.add("Soltero");
        datosPersonales.add("Calle San Fernando");

        System.out.println("Datos personales: " + datosPersonales);

        // 6. Crea un ArrayList llamado it_companies y asígnele los valores iniciales Facebook, Google, Microsoft, Apple, IBM, Oracle y Amazon.
        ArrayList<String> itCompanies = new ArrayList<>();
        itCompanies.add("Facebook");
        itCompanies.add("Google");
        itCompanies.add("Microsoft");
        itCompanies.add("Apple");
        itCompanies.add("IBM");
        itCompanies.add("Oracle");
        itCompanies.add("Amazon");

        // 7. Añadir una empresa a la lista it_companies utilizando la función add().
        itCompanies.add("NewCompany");

        System.out.println("Lista de empresas de tecnología: " + itCompanies);

        // 8. Comprobar si una determinada empresa existe en la lista it_companies.
        boolean existeEmpresa = itCompanies.contains("Google");
        System.out.println("¿Existe Google en la lista? " + existeEmpresa);

        // 9. Ordena la lista con el método sort()
        Collections.sort(itCompanies);
        System.out.println("Lista de empresas ordenada alfabéticamente: " + itCompanies);

        // 10. Invierte la lista en orden descendente utilizando el método reverse()
        Collections.reverse(itCompanies);
        System.out.println("Lista de empresas invertida: " + itCompanies);

        // 11. Elimina la primera empresa informática de la lista utilizando el método remove().
        itCompanies.remove("Facebook");

        System.out.println("Lista de empresas después de eliminar Facebook: " + itCompanies);

        // 12. Eliminar todas las empresas de la lista it_companies.
        itCompanies.clear();
        System.out.println("Lista de empresas después de eliminar todas: " + itCompanies);
    }
}
