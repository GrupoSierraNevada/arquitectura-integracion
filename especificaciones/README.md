#  Especificaciones

Algunas especificaciones técinas por parte y parte
Van primero los documentos de "conectores" que provee Domicilios.com
Eventualmente agregamos especificaciones de domicilios.com necesarias o de Grupo Sierra.

[Documento Descripcion del servicio REST](https://docs.google.com/document/d/1ZTf4hc82B3Xkz9Sx9-IuD1niZoWd2gTp4tgeMuB9X9s/edit?usp=sharing)

[Documento de especificacion de conector](https://docs.google.com/spreadsheets/d/1v3rnfED1wb_mbQ6km-7E_hFuOW3V9CpsHa7FhkHbtvs/edit?usp=sharing)

# pregutnas especificacoin conector
     
     - ¿Qué funcion cumple el cantidad2, cómo se que es consistente?

     - En movimiento de venta prepparacion , tipo registro 2 que
     diferencia hay entre f9833_precio_uni_total  y f9833_precio_uni. acaso total no debe tomar en cuenta las cantidades del factor?

     - en Impuestos, hacen referencia a F472_vlr_uni, pero el campo que hay es f9832_vlr_uni. es este mismo?

     - en Venta, f9831_vlr_tot es el valor del descuento o el valor después del descuento?

     -en venta, f_referencia_item es obligatorio? acaso un item puede estar en mmas de una familia a la vez?

    - en descuento, en el atributo f9831_vlr_tot está especificado pero no está en el ejemplo xml. Hay un vlr_tot en impuestos, y hay otro suelto pero no se sabe para qué es.

    - movimietno aux 9838, cuándo se usa? para qué sirve? Por qué está aparte?


[Códigos Paises](https://drive.google.com/file/d/1ThkuGxAwuisEfzYZymna2C-Cs_e_m25W/view?usp=sharing)

[Códigos Municipios](https://drive.google.com/file/d/1RmvTgXdn0Y9PffQAwlGibAP7vbI2M4h_/view?usp=sharing)

------------------------------------------------------------------------------------------------------------------------------

Preguntas Domicilios.com

by @felipehernandezrocha

-    En cuanto al tag t9820_pdv_d_doctos nos podrían aclarar que información puede o debe viajar en los siguientes campos:
          
          f9823_id_cia="1" // Siempre es "1", es una constante ?

        Si dentro de estas variables existen algunas que siempre van a tener el mismo valor por favor indicarnos cuales son           para poderlas configurar como constantes en nuestra plataforma.
        
-     En cuanto al tag  t9830_pdv_d_movto_venta nos podrían aclarar que información puede o debe viajar en los siguientes           campos:

              f_id_familia="Corral parrilla" // hace referencia al nombre del producto ?
              f9830_id_concepto="1201" // a que hace referencia esta variable ?
              f9830_id_unidad_medida="UNI " // cuales son las posibles unidades de medida ?
              f9834_tipo_familia_item="0" // a que hace referencia esta variable, siempre va en 0 ?
              f9834_tipo_reg_preparacion="0" // // a que hace referencia esta variable, siempre va en 0 ?
         
         Si dentro de estas variables existen algunas que siempre van a tener el mismo valor por favor indicarnos cuales son            para poderlas configurar como constantes en nuestra plataforma.

-     En cuanto al tag  t9832_pdv_d_movto_venta_impto nos podrían aclarar que información puede o debe viajar en los                 siguientes campos:

              f9832_id_llave_impuesto="019" // Es el porcentaje del IVA vigente verdad ?
              f9832_porcentaje_base="100.0000" // Es una constante ?
              f9832_tasa="19.0000" // Es el porcentaje del IVA vigente verdad ?
              f9832_vlr_uni="0.0000" // Es una constante ?
              f9832_vlr_tot="3752.0000" // A que hace referencia este campo ?
              f9832_ind_accion="1" // A que hace referencia este campo ? , es una constante ?
              f9832_ind_calculo="1"// A que hace referencia este campo ?, es una constante ?
         
         Si dentro de estas variables existen algunas que siempre van a tener el mismo valor por favor indicarnos cuales son            para poderlas configurar como constantes en nuestra plataforma.
         
           f_id_familia="Preparacion ceviches" // la famila es el nombre del extra que se esta adicionando ?
           f9833_tipo_registro="2" // Es una constante ?
           f9833_id_unidad_medida="UND " // nos pueden por favor enviar la tabla de unidades para homologarlas con las                                                     unidades de medida que manejamos en nustra plataforma.
           f9833_factor="2.0000" 
           f9833_cant_base="1.0000" 
           f9833_cant_1="2.0000" 
           f9833_cant_2="0.0000" // Siempre viaja en 0 , a que hace referencia este campo?
           f9833_precio_uni="3500.0000" 
           f9833_precio_uni_total="3500.0000" //  f9833_precio_uni_total = f9833_precio_uni="3500.0000" *f9833_cant_1 ??
           
En general por favor indicarnos que tags son constantes para poderlas parametrizar en la integración.

         



        
   
