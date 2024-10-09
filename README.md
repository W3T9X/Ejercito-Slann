<?xml version="1.0" encoding="UTF-8"?>
<catalogue id="slannArmy" name="Ejército Slann" revision="2" battleScribeVersion="2.03">
  <sharedProfiles>
    <profile id="unitProfile" name="Estadísticas">
      <characteristic name="Movimiento" />
      <characteristic name="Habilidad de Armas" />
      <characteristic name="Habilidad de Proyectiles" />
      <characteristic name="Fuerza" />
      <characteristic name="Resistencia" />
      <characteristic name="Heridas" />
      <characteristic name="Iniciativa" />
      <characteristic name="Ataques" />
      <characteristic name="Liderazgo" />
    </profile>
  </sharedProfiles>
  <sharedSelectionEntries>
    <selectionEntry id="commanderSlann" name="Mago Sacerdote Slann" type="unit">
      <profiles>
        <profile id="commanderSlannProfile" typeId="unitProfile" name="Estadísticas">
          <characteristic name="Movimiento" value="4" />
          <characteristic name="Habilidad de Armas" value="3" />
          <characteristic name="Habilidad de Proyectiles" value="0" />
          <characteristic name="Fuerza" value="3" />
          <characteristic name="Resistencia" value="5" />
          <characteristic name="Heridas" value="4" />
          <characteristic name="Iniciativa" value="2" />
          <characteristic name="Ataques" value="1" />
          <characteristic name="Liderazgo" value="9" />
        </profile>
      </profiles>
      <rules>
        <rule id="specialSave" name="Salvación Especial 4+">
          <description>El Mago Sacerdote Slann tiene una salvación especial de 4+.</description>
        </rule>
        <rule id="telepathy" name="Telepatía">
          <description>El Mago Sacerdote puede lanzar hechizos desde su aprendiz o el Altar de Guerra.</description>
        </rule>
        <rule id="protectedByAncestors" name="Protegido por los Ancestrales">
          <description>El Mago Sacerdote Slann tiene una salvación especial mejorada de 4+, otorgada por los Ancestrales.</description>
        </rule>
      </rules>
      <categories>
        <categoryLink id="commander" />
      </categories>
      <selectionEntries>
        <selectionEntryGroup id="options" name="Opciones Extra">
          <selectionEntry id="improveGeneration" name="Mejorar Generación" type="upgrade">
            <profiles>
              <profile id="improveGenerationProfile" name="Cuarta Generación">
                <characteristic name="Coste" value="+30" />
                <rule id="extraPower" name="+2 en Disfunciones Mágicas" />
              </profile>
            </profiles>
          </selectionEntry>
        </selectionEntryGroup>
        <selectionEntry id="magicalItems" name="Objetos Mágicos">
          <selectionEntryGroup id="magicalWeapons" name="Armas Mágicas">
            <selectionEntry id="swordOfSun" name="Espada del Sol Llameante" type="upgrade">
              <profiles>
                <profile id="magicSwordProfile" name="Espada del Sol Llameante">
                  <rule id="flamingAttacks" name="Ataques Flamígeros" />
                </profile>
              </profiles>
              <costs>
                <cost name="Coste" value="45" />
              </costs>
            </selectionEntry>
          </selectionEntryGroup>
          <selectionEntryGroup id="magicalArmors" name="Armaduras Mágicas">
            <selectionEntry id="armorOfAlligator" name="Armadura de Aligator" type="upgrade">
              <profiles>
                <profile id="armorOfAlligatorProfile" name="Armadura de Aligator">
                  <rule id="armorSave" name="Salvación por Armadura 4+" />
                </profile>
              </profiles>
              <costs>
                <cost name="Coste" value="20" />
              </costs>
            </selectionEntry>
          </selectionEntryGroup>
          <selectionEntryGroup id="magicalTalismans" name="Talismanes">
            <selectionEntry id="amuletOfProtection" name="Amuleto de Protección" type="upgrade">
              <profiles>
                <profile id="amuletOfProtectionProfile" name="Amuleto de Protección">
                  <rule id="wardSave" name="Salvación Especial 5+" />
                </profile>
              </profiles>
              <costs>
                <cost name="Coste" value="25" />
              </costs>
            </selectionEntry>
          </selectionEntryGroup>
        </selectionEntry>
      </selectionEntries>
    </selectionEntry>
    <selectionEntry id="warlordSlann" name="Caudillo Slann" type="unit">
      <profiles>
        <profile id="warlordSlannProfile" typeId="unitProfile" name="Estadísticas">
          <characteristic name="Movimiento" value="4" />
          <characteristic name="Habilidad de Armas" value="5" />
          <characteristic name="Habilidad de Proyectiles" value="2" />
          <characteristic name="Fuerza" value="4" />
          <characteristic name="Resistencia" value="5" />
          <characteristic name="Heridas" value="3" />
          <characteristic name="Iniciativa" value="4" />
          <characteristic name="Ataques" value="3" />
          <characteristic name="Liderazgo" value="9" />
        </profile>
      </profiles>
      <rules>
        <rule id="specialSave" name="Salvación Especial 5+">
          <description>El Caudillo Slann tiene una salvación especial de 5+.</description>
        </rule>
        <rule id="exampleToFollow" name="Ejemplo a Seguir">
          <description>El Caudillo Slann otorga a las unidades cercanas un bonificador de +1 para impactar en combate cuerpo a cuerpo.</description>
        </rule>
        <rule id="protectedByAncestors" name="Protegido por los Ancestrales">
          <description>El Caudillo Slann tiene una salvación especial mejorada de 5+, otorgada por los Ancestrales.</description>
        </rule>
      </rules>
      <categories>
        <categoryLink id="commander" />
      </categories>
      <selectionEntries>
        <selectionEntryGroup id="warriorType" name="Tipo de Guerrero">
          <selectionEntry id="jaguarWarrior" name="Guerrero Jaguar" type="upgrade">
            <costs>
              <cost name="Coste" value="+10" />
            </costs>
          </selectionEntry>
          <selectionEntry id="eagleWarrior" name="Guerrero Águila" type="upgrade">
            <costs>
              <cost name="Coste" value="+15" />
            </costs>
          </selectionEntry>
          <selectionEntry id="alligatorWarrior" name="Guerrero Aligator" type="upgrade">
            <costs>
              <cost name="Coste" value="+20" />
            </costs>
          </selectionEntry>
          <selectionEntry id="venomTribes" name="Venom Tribes" type="upgrade">
            <costs>
              <cost name="Coste" value="+10" />
            </costs>
          </selectionEntry>
          <selectionEntry id="warriorPriest" name="Sacerdote Guerrero" type="upgrade">
            <costs>
              <cost name="Coste" value="+15" />
            </costs>
          </selectionEntry>
        </selectionEntryGroup>
        <selectionEntry id="magicalItems" name="Objetos Mágicos">
          <selectionEntryGroup id="magicalWeapons" name="Armas Mágicas">
            <selectionEntry id="obsidianScythe" name="Guadaña de Obsidiana" type="upgrade">
              <profiles>
                <profile id="obsidianScytheProfile" name="Guadaña de Obsidiana">
                  <rule id="magicalAttacks" name="Ataques Mágicos" />
                </profile>
              </profiles>
              <costs>
                <cost name="Coste" value="35" />
              </costs>
            </selectionEntry>
          </selectionEntryGroup>
          <selectionEntryGroup id="magicalArmors" name="Armaduras Mágicas">
            <selectionEntry id="armorOfAlligator" name="Armadura de Aligator" type="upgrade">
              <profiles>
                <profile id="armorOfAlligatorProfile" name="Armadura de Aligator">
                  <rule id="armorSave" name="
