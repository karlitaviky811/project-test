<template>
  <v-container
    id="regular-tables"
    fluid
    tag="section"
  >
    <div class="py-3" />
     
    <base-material-card
      color="success"
      icon="mdi-clipboard-plus"
      title="Table on Dark Background"
      class="px-5 py-3"
    >
     <v-container class="d-flex flex-column align-end">
        <v-row>
            <v-col>
              <v-tooltip left>
                <template v-slot:activator="{ on: tooltip }">
                  <v-btn
                    v-on="{ ...tooltip }"
                    fab
                    small
                    v-show="true"
                    color="success"
                    @click.stop="create(true)"
                  >
                    <v-icon dark>mdi-plus</v-icon>
                  </v-btn>
                
                </template>
                <span>Nuevo</span>
              </v-tooltip>
            </v-col>
          </v-row>
     </v-container>
      <v-simple-table>
        <thead>
          <tr>
            <th class="primary--text">
              ID
            </th>
            <th class="primary--text">
              Nombre
            </th>
            <th class="primary--text">
              Tecnologias
            </th>
            <th class="primary--text">
              Departamento
            </th>
            <th class="primary--text">
              Responsable
            </th>
            <th class="text-right primary--text">
              Solicitudes
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1</td>
            <td>Dakota Rice</td>
            <td>Niger</td>
            <td>Oud-Turnhout</td>
            <td>Oud-Turnhout</td>
            <td class="text-right">
              $36,738
            </td>
          </tr>

          <tr>
            <td>2</td>
            <td>Minverva Hooper</td>
            <td>Curaçao</td>
            <td>Sinaas-Waas</td>
            <td>Sinaas-Waas</td>
            <td class="text-right">
              $23,789
            </td>
          </tr>

          <tr>
            <td>3</td>
            <td>Sage Rodriguez</td>
            <td>Netherlands</td>
            <td>Baileux</td>
              <td>Baileux</td>
            <td class="text-right">
              $56,142
            </td>
          </tr>

          <tr>
            <td>4</td>
            <td>Philip Chaney</td>
            <td>Korea, South</td>
            <td>Overland Park</td>
            <td>Overland Park</td>
            <td class="text-right">
              $38,735
            </td>
          </tr>

          <tr>
            <td>5</td>
            <td>Doris Greene</td>
            <td>Malawi</td>
            <td>Feldkirchen in Kärnten</td>
            <td>Feldkirchen in Kärnten</td>
            <td class="text-right">
              $63,542
            </td>
          </tr>

          <tr>
            <td>6</td>
            <td>Mason Porter</td>
            <td>Chile</td>
            <td>Gloucester</td>
            <td>Gloucester</td>
            <td class="text-right">
              $78,615
            </td>
          </tr>
        </tbody>
      </v-simple-table>
    </base-material-card>
  </v-container>
</template>
