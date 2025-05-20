
# PREMIS Data Dictionary Version 2.1: Hierarchical Listing of Semantic Units

<p>The PREMIS Data Dictionary and its supporting documentation is a comprehensive,
          practical resource for implementing preservation metadata in digital
          archiving systems. The Data Dictionary is built on a data model that
          defines five entities: Intellectual Entities, Objects, Events, Rights,
          and Agents. Each semantic unit defined in the Data Dictionary is a
          property of one of the entities in the data model.</p>

<p>This is a hierarchical listing of the semantic units included in the
          Data Dictionary. The information in parentheses following each semantic
          unit indicates whether the element is Mandatory (M) or Optional (O),
          followed by whether it is Repeatable (R) or Not repeatable (NR). Some
          semantic units in the Object section are further divided by the types
          of representation, file, and bitstream. Where not qualified, the designations
          apply to all three types. Where qualified, only the types listed are
          applicable.</p>


## 1. Object
<ul>
          <li>1.1	objectIdentifier (M, R)
            <ul>

              <li>1.1.1 objectIdentifierType (M, NR)</li>

              <li>1.1.2 objectIdentifierValue (M, NR)</li>
            </ul>
          </li>
          <li>1.2	objectCategory (M, NR)</li>
          <li>1.3	preservationLevel (O, R) [representation, file]
            <ul>

              <li>1.3.1 preservationLevelValue (M, NR) [representation, file]</li>
              <li>1.3.2 preservationLevelRole (O, NR) [representation, file]</li>

              <li>1.3.3 preservationLevelRationale (O, R) [representation, file]</li>
              <li>1.3.4 preservationLevelDateAssigned (O, NR) [representation, file]</li>
            </ul>
          </li>

          <li>1.4	significantProperties (O, R)
            <ul>
              <li>1.4.1 significantPropertiesType (O, NR)</li>
              <li>1.4.2 significantPropertiesValue (O, NR)</li>
              <li>1.4.3 significantPropertiesExtension (O, R)</li>
            </ul>
          </li>
          <li>1.5	objectCharacteristics (M, R) [file, bitstream]
            <ul>

              <li>1.5.1 compositionLevel (M, NR) [file, bitstream]</li>
              <li>1.5.2 fixity (O, R) [file, bitstream]
                <ul>
                  <li>1.5.2.1	messageDigestAlgorithm (M, NR) [file, bitstream]</li>
                  <li>1.5.2.2	messageDigest (M, NR) [file, bitstream]</li>
                  <li>1.5.2.3	messageDigestOriginator (O, NR) [file, bitstream]</li>
                </ul>

              </li>
              <li>1.5.3 size (O, NR) [file, bitstream]</li>
              <li>1.5.4 format (M, R) [file, bitstream]
                <ul>
                  <li>1.5.4.1	formatDesignation (O, NR) [file, bitstream]
                    <ul>
                      <li>1.5.4.1.1 formatName (M, NR) [file, bitstream]</li>
                      <li>1.5.4.1.2 formatVersion (O, NR) [file, bitstream]</li>

                    </ul>
                  </li>
                  <li>1.5.4.2	formatRegistry (O, NR) [file, bitstream]
                    <ul>
                      <li>1.5.4.2.1 formatRegistryName (M, NR) [file, bitstream]</li>
                      <li>1.5.4.2.2 formatRegistryKey (M, NR) [file, bitstream]</li>
                      <li>1.5.4.2.3 formatRegistryRole (O, NR) [file, bitstream]</li>
                    </ul>

                  </li>
                  <li>v1.5.4.3 formatNote (O, R) [file, bitstream]</li>
                </ul>
              </li>
              <li>1.5.5 creatingApplication (O, NR) [file, bitstream]
                <ul>
                  <li>1.5.5.1	creatingApplicationName (O, NR) [file, bitstream]</li>
                  <li>1.5.5.2	creatingApplicationVersion (O, NR) [file, bitstream]</li>

                  <li>1.5.5.3	dateCreatedByApplication (O, NR) [file, bitstream]</li>
                  <li>1.5.5.4	creatingApplicationExtension (O, R) [file, bitstream]</li>
                </ul>
              </li>
              <li>1.5.6 inhibitors (O, R) [file, bitstream]
                <ul>
                  <li>1.5.6.1	inhibitorType (M, NR) [file, bitstream]</li>
                  <li>1.5.6.2	inhibitorTarget (O, R) [file, bitstream]</li>

                  <li>1.5.6.3	inhibitorKey (O, NR) [file, bitstream]</li>
                </ul>
              </li>
              <li>1.5.7 objectCharacteristicsExtension (O, R) [file, bitstream]</li>
            </ul>
          </li>
          <li>1.6	originalName (O, NR) [representation, file]</li>

          <li>1.7	storage (O, R) [file, bitstream]
            <ul>
              <li>1.7.1 contentLocation (O, NR) [file, bitstream]
                <ul>
                  <li>1.7.1.1	contentLocationType (M, NR) [file, bitstream]</li>
                  <li>1.7.1.2	contentLocationValue (M, NR) [file, bitstream]</li>

                </ul>
              </li>

              <li>1.7.2 storageMedium (O, NR) [file, bitstream]</li>
            </ul>
          </li>
          <li>1.8	environment (O, R)
            <ul>
              <li>1.8.1 environmentCharacteristic (O, NR)</li>

              <li>1.8.2 environmentPurpose (O, R)</li>

              <li>1.8.3 environmentNote (O, R)</li>
              <li>1.8.4 dependency (O, R)
                <ul>
                  <li>1.8.4.1	dependencyName (O, R)</li>
                  <li>1.8.4.2	dependencyIdentifier (O, R)
                    <ul>
                      <li>1.8.4.2.1 dependencyIdentifierType (M, NR)</li>
                      <li>1.8.4.2.2 dependencyIdentifierValue (M, NR)</li>

                    </ul>
                  </li>
                </ul>
              </li>
              <li>1.8.5 software (O, R)
                <ul>
                  <li>1.8.5.1	swName (M, NR)</li>
                  <li>1.8.5.2	swVersion (O, NR)</li>

                  <li>1.8.5.3	swType (M, NR)</li>
                  <li>1.8.5.4	swOtherInformation (O, R)</li>
                  <li>1.8.5.5	swDependency (O, R)</li>
                </ul>
              </li>
              <li>1.8.6 hardware (O, R)
                <ul>
                  <li>1.8.6.1	hwName (M, NR)</li>

                  <li>1.8.6.2	hwType (M, NR)</li>
                  <li>1.8.6.3	hwOtherInformation (O, R)</li>
                </ul>
              </li>
              <li>1.8.7 environmentExtension (O, R)</li>
            </ul>

          </li>

          <li>1.9	signatureInformation (O, R) [file, bitstream]
            <ul>
              <li>1.9.1 signature (O, R)
                <ul>
                  <li>1.9.1.1	signatureEncoding (M, NR) [file, bitstream]</li>
                  <li>1.9.1.2	signer (O, NR) [file, bitstream]</li>
                  <li>1.9.1.3	signatureMethod (M, NR) [file, bitstream]</li>
                  <li>1.9.1.4	signatureValue (M, NR) [file, bitstream]</li>

                  <li>1.9.1.5	signatureValidationRules (M, NR) [file, bitstream]</li>
                  <li>1.9.1.6	signatureProperties (O, R) [file, bitstream]</li>
                  <li>1.9.1.7	keyInformation (O, NR) [file, bitstream]</li>
                </ul>
              </li>
              <li>1.9.2 signatureInformationExtension (O, R) [file, bitstream]</li>
            </ul>

          </li>
          <li>1.10 relationship (O, R)
            <ul>
              <li>1.10.1 relationshipType (M, NR)</li>
              <li>1.10.2 relationshipSubType (M, NR)</li>
              <li>1.10.3 relatedObjectIdentification (M, R)
                <ul>
                  <li>1.10.3.1 relatedObjectIdentifierType (M, NR)</li>

                  <li>1.10.3.2 relatedObjectIdentifierValue (M, NR)</li>
                  <li>1.10.3.3 relatedObjectSequence (O, NR)</li>
                </ul>
              </li>
              <li>1.10.4 relatedEventIdentification (O, R)
                <ul>
                  <li>1.10.4.1 relatedEventIdentifierType (M, NR)</li>
                  <li>1.10.4.2 relatedEventIdentifierValue (M, NR)</li>

                  <li>1.10.4.3 relatedEventSequence (O, NR)</li>
                </ul>
              </li>
            </ul>
          </li>
          <li>1.11 linkingEventIdentifier (O, R)
            <ul>
              <li>1.11.1 linkingEventIdentifierType (M, NR)</li>

              <li>1.11.2 linkingEventIdentifierValue (M, NR)</li>
            </ul>
          </li>
          <li>1.12 linkingIntellectualEntityIdentifier (O, R)
            <ul>
              <li>1.12.1 linkingIntellectualEntityIdentifierType (M, NR)</li>
              <li>1.12.2 linkingIntellectualEntityIdentifierValue (M, NR)</li>

            </ul>
          </li>
          <li>1.13 linkingRightsStatementIdentifier (O, R)
            <ul>
              <li>1.13.1 linkingRightsStatementIdentifierType (M, NR)</li>
              <li>1.13.2 linkingRightsStatementIdentifierValue (M, NR)</li>
            </ul>
          </li>

        </ul>

## 2. Event
<ul>
          <li>2.1	eventIdentifier (M, NR)
            <ul>
              <li>2.1.1 eventIdentifierType (M, NR)</li>
              <li>2.1.2 eventIdentifierValue (M, NR)</li>

            </ul>
          </li>

          <li>2.2	eventType (M, NR)</li>
          <li>2.3	eventDateTime (M, NR)</li>
          <li>2.4	eventDetail (O, NR)</li>
          <li>2.5	eventOutcomeInformation (O, R)
            <ul>

              <li>2.5.1 eventOutcome (O, NR)</li>
              <li>2.5.2 eventOutcomeDetail (O, R)
                <ul>
                  <li>2.5.2.1	eventOutcomeDetailNote (O, NR)</li>
                  <li>2.5.2.2	eventOutcomeDetailExtension (O, R)</li>
                </ul>
              </li>
            </ul>

          </li>
          <li>2.6	linkingAgentIdentifier (O, R)
            <ul>
              <li>2.6.1 linkingAgentIdentifierType (M, NR)</li>
              <li>2.6.2 linkingAgentIdentifierValue (M, NR)</li>
              <li>2.6.3 linkingAgentRole (O, R)</li>
            </ul>
          </li>

          <li>2.7	linkingObjectIdentifier (O, R)
            <ul>
              <li>2.7.1 linkingObjectIdentifierType (M, NR)</li>
              <li>2.7.2 linkingObjectIdentifierValue (M, NR)</li>
              <li>2.7.3 linkingObjectRole (O, R)</li>
            </ul>
          </li>
        </ul>

## 3. Agent
<ul>
          <li>3.1	agentIdentifier (R, M)
            <ul>
              <li>3.1.1 agentIdentifierType (M, NR)</li>
              <li>3.1.2 agentIdentifierValue (M, NR)</li>
            </ul>
          </li>

          <li>3.2	agentName (O, R)</li>
          <li>3.3	agentType (O, NR)</li>
					<li>3.4 agentNote (O, R)</li>
					<li>3.5 agentExtension (O, R)</li>
					<li>3.6 linkingEventIdentifier (O, R)
					<ul>
							<li>3.6.1 linkingEventIdentifierType (M, NR)</li>

							<li>3.6.2 linkingEventIdentifierValue (M, NR)</li>
            </ul>
          </li>
					<li>3.7 linkingRightsStatementIdentifier (O, R)
					<ul>
								<li>3.7.1 linkingRightsStatementIdentifierType (M, NR)</li>
								<li>3.7.2 linkingRightsStatementIdentifierValue (M, NR)</li>
				</ul>

				</li>				
        </ul>

## 4. Rights
<ul>
          <li>4.1	rightsStatement (O, R)
            <ul>
              <li>4.1.1 rightsStatementIdentifier (M, NR)
                <ul>
                  <li>4.1.1.1	rightsStatementIdentifierType (M, NR)</li>

                  <li>4.1.1.2	rightsStatementIdentifierValue (M, NR)</li>

                </ul>
              </li>
              <li>4.1.2 rightsBasis (M, NR)</li>
              <li>4.1.3 copyrightInformation (O, NR)
                <ul>
                  <li>4.1.3.1	copyrightStatus (M, NR)</li>

                  <li>4.1.3.2	copyrightJurisdiction (M, NR)</li>
                  <li>4.1.3.3	copyrightStatusDeterminationDate (O, NR)</li>

                  <li>4.1.3.4	copyrightNote (O, R)</li>
                </ul>
              </li>
              <li>4.1.4 licenseInformation (O, NR)
                <ul>

                  <li>4.1.4.1	licenseIdentifier (O, NR)
                    <ul>
                      <li>4.1.4.1.1 licenseIdentifierType (M, NR)</li>
                      <li>4.1.4.1.2 licenseIdentifierValue (M, NR)</li>

                    </ul>
                  </li>
                  <li>4.1.4.2	licenseTerms (O, NR)</li>

                  <li>4.1.4.3	licenseNote (O, R)</li>
                </ul>
              </li>
              <li>4.1.5 statuteInformation (O, R)
                <ul>

                  <li>4.1.5.1	statuteJurisdiction (M, NR)</li>
                  <li>4.1.5.2	statuteCitation (M, NR)</li>

                  <li>4.1.5.3	statuteInformationDeterminationDate (O, NR)</li>
                  <li>4.1.5.4	statuteNote (O, R)</li>
                </ul>
              </li>
              <li>4.1.6 rightsGranted (O, R)
                <ul>

                  <li>4.1.6.1	act (M, NR)</li>

                  <li>4.1.6.2	restriction (O, R)</li>
                  <li>4.1.6.3	termOfGrant (M, NR)
                    <ul>
                      <li>4.1.6.3.1 startDate (M, NR)</li>
                      <li>4.1.6.3.2 endDate (O, NR)</li>
                    </ul>

                  </li>

                  <li>4.1.6.4	rightsGrantedNote (O, R)</li>
                </ul>
              </li>
              <li>4.1.7 linkingObjectIdentifier (O, R)
                <ul>
                  <li>4.1.7.1	linkingObjectIdentifierType (M, NR)</li>
                  <li>4.1.7.2	linkingObjectIdentifierValue (M, NR)</li>
                  <li>4.1.7.3 linkingObjectRole (O, R)</li>

                </ul>
              </li>
              <li>4.1.8 linkingAgentIdentifier (O, R)
                <ul>
                  <li>4.1.8.1	linkingAgentIdentifierType (M, NR)</li>
                  <li>4.1.8.2	linkingAgentIdentifierValue (M, NR)</li>
                  <li>4.1.8.3	linkingAgentRole (O, NR)</li>
                </ul>

              </li>
							<li>4.2 rightsExtension (O, R)</li>
            </ul>
          </li>
          <li>4.2	rightsExtension (O, R)</li>
        </ul>
