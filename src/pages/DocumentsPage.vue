<template>
  <div class="c-container">
    <q-splitter
      v-model="splitterModel"
      style="height: 850px"

    >

      <template v-slot:before>
        <q-tabs
          v-model="tab"
          vertical
          class="text-teal"
        >
          <q-tab name="policy" icon="policy" label="Privacy Policy" />
          <q-tab name="terms" icon="gavel" label="Terms of use" />
          <q-tab name="aml" icon="account_circle" label="AML/KYC" />
          <q-tab name="regulations" icon="assured_workload" label="Regulations" />
          <q-tab name="rules" icon="rule" label="Rules" />
        </q-tabs>
      </template>

      <template v-slot:after>
        <q-tab-panels
          v-model="tab"
          animated
          swipeable
          vertical
          transition-prev="jump-up"
          transition-next="jump-up"
        >
          <q-tab-panel name="policy">
            <div class="text-h4 q-mb-md">Privacy Policy</div>
            <p>


              Effective date: 01.05.22.

              This Privacy Policy (hereinafter referred to as the Policy) defines the policy regarding the processing of personal data, contains information on the implemented requirements for the protection of the Operator's personal data.
              1. Terms and definitions

              1.1. Data subject - an individual who has reached the age of majority using the Site on the Internet y-swap.com for financial transactions with electronic, digital or fiat currency.

              1.2. Cookies - a piece of data as part of an HTTPS request, intended for storage on the Subject's end device and used by the Operator to identify the Subject.

              1.3. Site - a set of programs for electronic computers and other information in the information and telecommunications network "Internet", designed to be displayed in a browser and accessed using the domain name of the Operator. In the context of the Operator's activities, the site y-swap.com is used

              1.4. Registration data - a list of information specified by the Operator when registering on the y-swap.com website, and later when they change during the execution of the contract.

              1.5. Processing of personal data - any action (operation) or a set of actions (operations) performed using automation tools or without using such tools with personal data, including collection, recording, systematization, accumulation, storage, clarification (updating, changing), extraction, use, transfer (distribution, provision, access), blocking, deletion, destruction of personal data.
              2. General provisions

              2.1. The Policy regulates the processing of personal data when the Operator carries out business activities, including the provision of services for the purchase/sale for the User and on behalf of the User of electronic and/or digital or fiat currency.

              2.2. The requirements for the security of personal data transferred between the Operator and the Subjects are provided for by the agreement (User Agreement) concluded between them in accordance with applicable law.

              2.3. In a situation where personal data is received from the Personal Data Subject, the latter is responsible for indicating false personal data.

              2.4. This Policy applies to personal data received both before and after the entry into force of this Policy.

              2.5. The operator is obliged to adhere to the following principles when processing personal data:

              2.5.1. the processing of personal data must be carried out on a lawful and fair basis;

              2.5.2. the processing of personal data should be limited to the achievement of specific, predetermined and legitimate purposes. It is not allowed to process personal data that is incompatible with the purposes of collecting personal data;

              2.5.3. it is not allowed to combine databases containing personal data, the processing of which is carried out for purposes that are incompatible with each other;

              2.5.4. only personal data that meet the purposes of their processing are subject to processing;

              2.5.5. the content and scope of the processed personal data must correspond to the stated purposes of processing. The processed personal data should not be excessive in relation to the stated purposes of their processing;

              2.5.6. when processing personal data, the accuracy of personal data, their sufficiency, and, if necessary, relevance in relation to the purposes of processing personal data, must be ensured.

              2.5.7. storage of personal data should be carried out in a form that allows determining the subject of personal data, no longer than required by the purposes of processing personal data, unless the period for storing personal data is established by federal law, an agreement to which the subject of personal data is a party, beneficiary or guarantor. The processed personal data is subject to destruction or depersonalization upon reaching the goals of processing or in case of loss of the need to achieve these goals, unless otherwise provided by federal law.

              2.5. This Policy is published on the Internet on the website y-swap.com.
              3. Categories of personal data subjects

              3.1. The Operator processes the personal data of all Data Subjects who are Users of the y-swap.com website.
              4. Purposes and grounds for the processing of personal data

              4.1. The personal data of the Subjects regarding the use of the Site are processed to achieve the following purposes:

              4.1.1. familiarization of the User with the services of the Operator;

              4.1.2. conclusion of an agreement between the User and the Operator and for the purpose of its execution;

              4.1.3. notification of Users about changes in the operation of the Operator's Service,

              4.1.4. providing support and service to Users of the Service;

              4.1.5. to monitor the use of the Service

              4.2. The personal data of the Subjects are processed in connection with the performance of services for the purchase / sale for the User and on behalf of the User of electronic throne and/or digital or fiat currency.

              4.3. Personal data may be used for other purposes, if this is mandatory in accordance with the provisions of the current legislation.

              4.4. The processing of personal data is limited to the achievement of specific, predetermined and legitimate purposes. It is not allowed to process personal data that is incompatible with the purposes of collecting personal data.
              5. Composition of information about personal data subjects

              5.1. The Operator has the right to process the following categories of personal data of the Subjects: name, age, passport data, bank card number, electronic payment system account number, cryptocurrency wallet address, e-mail, telephone number, address (house, street, town, country), cookies .

              5.2. The period of storage of personal data is determined by the contract or the nature of another basis for processing.

              5.3. The term for processing the personal data of the Subjects is until the end of the provision of services for the purchase / sale for the User and on behalf of the User of electronic and / or digital or fiat currency.

              5.4. The term for processing the personal data of the Subjects after the provision of the services specified in clause 5.3 is within 3 years.

              5.5. Storage of material carriers of personal data is carried out separately for each category of personal data subjects.
              6. Storage and processing of personal data

              6.1. The operator may process personal data in personal data information systems, ensuring their proper protection.
              7. Rights of the Subject

              The subject of personal data has the right:

              7.1. Apply for changes to the provided personal data or for their deletion.

              7.2. Send requests to the Operator regarding the processing of his personal data, within the competence of the Operator.

              7.3. Exercise other rights provided for by applicable law.

              7.4. Apply for changes to the provided personal data or for their deletion. Send requests to the Operator regarding the processing of his personal data within the competence of the Operator. Exercise other rights provided for by applicable law.
              8. Information on the implemented requirements for the protection of personal data

              8.1. When processing personal data, the Operator takes the necessary legal, organizational and technical measures and ensures their adoption to protect personal data from unauthorized or accidental access to them, destruction, modification, blocking, copying, provision, distribution of personal data, as well as from other illegal actions in in relation to personal data, which are in particular (but not limited to):

              8.2. Appointment of a person responsible for the processing of personal data.

              8.3. Limiting the composition of employees with access to personal data.

              8.4. Software identification of the Subjects, employees of the Operator and accounting of their actions.

              8.5. Implementation of anti-virus control and other measures against malicious software and mathematical impact.

              8.6. Application of backup and recovery tools.

              8.7. Update software when vendor-specific security patches are available.

              8.8. Implementation of encryption when transferring personal data on the Internet.

              8.9. Taking measures related to the admission of only appropriate persons in the places of installation of technical means.

              8.10. The use of technical means of protection of the premises in which the technical means of information systems of personal data are located, and places of storage of material carriers of personal data.

              8.11. The operator ensures the security of personal data, in particular by using them:

              8.11.1. taking into account the possible harm to the subject of personal data, the volume and content of the processed personal data, the type of activity in which personal data is processed, the relevance of threats to the security of personal data;

              8.11.2. application of technical measures in accordance with threats to the security of personal data during their processing in personal data information systems;

              8.11.3. with the use of organizational and technical measures to ensure the security of personal data during their processing in information systems necessary to comply with the requirements of legislation on the protection of personal data;

              8.11.4. using information security tools that have passed the conformity assessment procedure in the prescribed manner;

              8.11.5. with an assessment of the effectiveness of the measures taken to ensure the security of personal data before starting work in the personal data information system;

              8.11.6. taking into account machine carriers of personal data, if they are used;

              8.11.7. with the application of procedures related to the detection of facts of unauthorized access to personal data and the adoption of measures;

              8.11.8. with the possibility of recovering personal data modified or destroyed due to unauthorized access to them;

              8.11.9. with the establishment of access rules to personal data processed in the personal data information system, as well as ensuring the registration and accounting of all actions performed with them;

              8.11.10. with control over the measures taken to ensure the security of personal data and the level of security of personal data information systems.
              9. Working with password protection

              9.1. Personal passwords must be generated by special administrative service software or created directly by the Subjects using the site during registration.

              9.2. The password must be at least 8 characters long.

              9.3. The password must contain upper and lower case letters, numbers and special characters.

              9.4. The password must not include:

              - easily calculated combinations of characters;

              − keyboard sequences of characters and signs;

              − generally accepted abbreviations;

              − abbreviations;

              phone numbers, cars;

              − other combinations of letters and signs associated with the Subject;

              - when changing the password, the new combination of characters must differ from the previous one by at least 2 characters.

              9.5. It is allowed to use a single password to obtain access by the Subject to various information resources.

              9.6. A complete unscheduled change of passwords for all Subjects must be performed in the event of the termination of the powers of administrators.

              9.7. A complete unscheduled change of passwords should be made in the event of a compromise of the personal password of one of the administrators.

              9.8. In case of compromise of the personal password of the Subject, it is necessary to immediately restrict access to information from this account, until the new account of the Subject or password takes effect.

              9.9. When working with password protection, Subjects are prohibited from:

              − disclose to anyone your personal password and other identifying information;

              - provide access from your account to information to unauthorized persons;

              - write down passwords on paper, file, electronic and other media, including objects.

              9.10. Storage by the Subject of his password on paper is allowed only in a personal safe sealed by the owner of the password.

              9.11. When entering a password, the Subject is obliged to exclude the possibility of its interception by third parties and technical means.

              9.12. Compromise means:

              − physical loss of the carrier with information;

              − transmission of identification information via open communication channels;

              − penetration of an unauthorized person into the premises of physical storage of the password information carrier or algorithm or suspicion of it (alarm operation, damage to UA control devices (imprints of seals), damage to locks, etc.);

              − visual inspection of the carrier of identification information by an unauthorized person;

              − interception of the password during the distribution of identifiers;

              − deliberate transfer of information to a third party.

              9.13. Actions in case of password compromise:

              − a compromised password is immediately disabled, and a spare or new password is entered instead;

              - all participants in the exchange of information are immediately notified about the compromise. The password is added to special lists containing compromised passwords and accounts.
              10. Privacy

              10.1. The operator and other persons who have gained access to personal data are obliged not to disclose to third parties and not to distribute personal data without observing the principle based on the consent of the subject of personal data, except as otherwise provided by applicable law.
              11. Destruction (depersonalization) of personal data

              11.1. Destruction (depersonalization) of the personal data of the Subject is carried out in the following cases:

              11.1.1. upon reaching the goals of their processing or in case of loss of the need to achieve them within a period not exceeding thirty days from the moment the goal of processing personal data is achieved, unless otherwise provided by the agreement to which the subject of personal data is a party, another agreement between the Operator and the subject of personal data (his representative, employer);

              11.1.2. in case of unlawful processing of personal data or lawful withdrawal of personal data within a period not exceeding ten working days from the date of detection of such a case;

              11.1.3. in the event of the expiration of the period of storage of personal data, determined in accordance with the legislation and organizational and administrative documents of the Operator;

              11.1.4. in the case of an order from the authorized body for the protection of the rights of personal data subjects, prosecution authorities or a court decision.
              12. Transfer to third parties

              12.1 The Operator may transfer personal data to other persons, hosting providers, analytics services, other persons in order to fulfill the contract concluded with third parties.

              12.2. The Operator guarantees the conclusion of an adequate order for the processing of personal data in the event that third parties are involved in accordance with the contractual powers of the Operator.

              12.3. The operator has the right to transfer personal data to the bodies of inquiry and investigation, other authorized bodies for grounds and in cases expressly provided for by applicable law.
              13. Final provisions

              13.1. The term for processing personal data processed by the Operator may be determined by the organizational and administrative documents of the Operator.

              13.2. This Policy is subject to change, addition in the event of the emergence of new legislative acts and special regulations on the processing and protection of personal data, as well as by decision of the Operator.

              13.3. Control over the fulfillment of the requirements of this Policy is carried out by the person responsible for organizing the processing of personal data.

              13.4. Issues not regulated by this Policy are regulated by the current legislation.

              13.5. The operator may issue other local acts that clarify certain principles for the processing of personal data.

            </p>
          </q-tab-panel>

          <q-tab-panel name="terms">
            <div class="text-h4 q-mb-md">Terms of use</div>
            <p>


              This agreement is located for public access on the Internet on the page y-swap.com and can be changed by the Service Manual unilaterally without additional notice to the User.

              The parties to this agreement are y-swap.com, hereinafter simply the "Service" and any individual using the services of the Service, hereinafter referred to as the "User".
              1. Terms and definitions

              1.1. y-swap.com is a trademark that is the name for a cryptocurrency exchange point and offers its services through a special software interface for all Users.

              1.2. A user is any natural person using the services of the y-swap.com service.

              1.3. Electronic currency is a monetary obligation between the developer of this currency and its user, expressed digitally.

              1.4. A payment system is a software and hardware product developed by a third party and is a mechanism for implementing the accounting of monetary obligations, as well as organizing mutual settlements between its users.

              1.5. Service Services - operations for depositing and withdrawing electronic currencies, as well as other services, information about which is posted on the Service window.

              1.6. Payment - transfer of electronic currency from the payer to the recipient.
              2. Introduction

              2.1. This agreement governs the relationship between the User and the Service regarding the services provided by the Service to the User and cancels all previous agreements between the Service and the User on this subject.

              2.2. This agreement does not cancel the current legislation of the countries of registration and location of the Service and the User, as well as the contractual relationship between the User and the Payment system (systems). If, under the terms of the current legislation or other agreements, the User cannot use the services of the Service, then the use of these services by the User is prohibited by these rules and will be recognized as illegal.

              2.3. The Service guarantees and ensures the confidentiality of information about the User and his operations. The Service can provide this information only at the request of authorized state bodies, officials or representatives of Payment systems, if there are legal grounds for this.
              3. Subject of the agreement

              3.1. The subject of this agreement are services for depositing and withdrawing electronic currencies, as well as other services, the description of which is given on the Service window.

              3.2. The Service offers its services to all Users and does not verify the eligibility and legality of the User's possession of electronic currencies and / or financial resources, and does not supervise the User's operations in any of the Payment systems.

              3.3. Payment systems and/or financial institutions are solely responsible for the funds entrusted to them by the User. The Service cannot be a party to an agreement between the Payment System and/or a financial institution and the User and is in no way responsible for the User's misuse or unauthorized use of the Payment System's capabilities, as well as for the User's abuse of the functionality of the Payment System. Mutual rights and obligations of the User and the Payment System and/or financial institution are governed by the relevant agreements.

              3.4. Any completed operation for depositing and withdrawing electronic currency, as well as any other operation offered by the Service to the User is considered irrevocable, i.e. cannot be canceled by the User after its completion - receipt by the User of what is due to him under previously accepted terms of the transaction.

              3.5. The Service has the right to suspend or cancel the operation in progress if the authorized bodies receive information about the incompetence of the User to own electronic currencies or financial resources and / or other information that makes it impossible for the Service to provide services to the User.

              3.6. The Service has the right to suspend or cancel the ongoing operation if the User violates the terms of this agreement.

              3.7. The Service has the right to cancel the operation in progress and return the electronic currencies and / or funds deposited by the User without explanation.

              3.8. The user undertakes:

              - exclude any possible complicity in illegal trade and any other illegal operations using the services of the Service;

              - exclude any possible complicity in financial fraud, do not use the Service to create and distribute pyramid schemes, as well as to perform other actions that are contrary to the law and legal norms;

              - exclude in their practical activities using the Service any actions, the implementation of which may cause direct or indirect harm to the fight against laundering and legalization of illegally obtained funds;

              3.9. The Service undertakes to take all possible and available actions to prevent attempts of illegal trading, financial fraud and money laundering using the services of the Service. These actions include but are not limited to:

              - provide all possible assistance to law enforcement agencies in the search and capture of financial terrorists engaged in illegal activities of money laundering.

              - providing the competent authorities, in accordance with applicable law, with information regarding the processing of the Service;

              - improving the Service to prevent direct or indirect use of the Service in activities that are contrary to legislation aimed at combating illegal trade, financial fraud and money laundering.
              4. Service services

              4.1. Ordering the services of the Service and obtaining information about the progress of the transaction by the User are made exclusively through contacts with a representative of the Service.

              4.2. The service offers its services without a break for lunch and will strive to ensure that services are provided seven days a week and around the clock.
              6. Refund

              Automatic or semi-automatic refund on our service is possible for the following reasons:

              6.1. As a result of an error made by the user when making an exchange on our service:

              6.1.1 Payment was made from a wallet other than the one specified in the exchange;

              6.1.2 The amount of the actual payment does not correspond to the one declared in the exchange (for more details, see clause 4.18 of the Site Rules);

              6.1.3 The exchange contains outdated mail or one that does not belong to the user;

              6.2. If it is impossible to transfer funds to the details specified by the user in the application, for such reasons as:

              6.2.1 The specified requisite is the number of the expired/invalid card;

              6.2.2 The specified details have reached the limit for depositing funds;

              6.2.3 The currency of the specified attribute is different from the one selected in the exchange direction;

              6.2.4 The User failed / refused to provide evidence of possession of the card with which the payment was made; When making a refund to the original requisite / wallet, the costs for the reverse transfer are paid by the user according to the current tariff of the payment system from which the payment was received on the request by the service.
              7. Taxation

              7.1. The Service is not a tax agent for the User and will not notify the User of his tax costs. The user undertakes to independently pay all taxes required by the tax legislation of his place of residence.

              7.2. In the event that the authorities require the Service to pay the User's taxes or cover the debt resulting from the User's refusal to pay taxes, the User agrees to reimburse the Service for all these payments.
              8. Guarantees and liability of the parties

              8.1. The Service provides its services on an "as is" basis as they are described on the pages of the Service's website and does not offer any additional warranties.

              8.2. The Service guarantees the fulfillment of obligations to the User only within the limits of the amounts entrusted to the Service by the User for the operation.

              8.3. The Service will make every effort, but does not guarantee that its services will be available around the clock and daily. The Service does not bear any responsibility for losses, lost profits and other costs of the User resulting from the impossibility of obtaining access to the site and services of the Service.

              8.4. The Service does not bear any responsibility for losses, lost profits and other costs of the User resulting from delays, errors or failures in making bank payments or electronic transfers.

              8.5. The Service does not bear any responsibility for losses, lost profits and other costs of the User, resulting from the User's erroneous expectations regarding the tariff rates of the Service, the profitability of transactions and other subjective factors.

              8.6. The User guarantees indemnification of the Service (management company, managers and employees) in cases of claims or claims directly or indirectly related to the User's use of the Service, with the exception of losses caused by the guilty (intentional or negligent) actions of the Service itself.

              8.7. The User guarantees that he is the owner or has legal grounds for the disposal of the amounts used in his transactions.

              8.8. The User undertakes not to falsify communication flows related to the functioning of the Service.

              8.9. The User acknowledges that the content of the Service website is protected by the laws on the protection of property rights, intellectual property and copyrights. Unauthorized use of this content is illegal.
              9. Force majeure

              9.1. Neither the User nor the Service will be liable to each other for delays or failure to fulfill their obligations resulting from the occurrence of force majeure circumstances, including natural disasters, fire, flood, terrorist attacks, power shifts, civil unrest, as well as non-functioning of Payment systems, energy supply systems , telecommunications and Internet service providers.

            </p>
          </q-tab-panel>

          <q-tab-panel name="aml">
            <div class="text-h4 q-mb-md">AML/KYC</div>
            <p>ccccccc</p>

          </q-tab-panel>


        <q-tab-panel name="regulations">
          <div class="text-h4 q-mb-md">Regulations</div>
          <p>xxxxxxx</p>
        </q-tab-panel>

        <q-tab-panel name="rules">
          <div class="text-h4 q-mb-md">Rules</div>
          <p>nnnnnnnnn</p>
        </q-tab-panel>
        </q-tab-panels>
      </template>

    </q-splitter>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  name: "DocumentsPage",
  setup() {
    return {
      tab: ref('policy'),
      splitterModel: ref(20)
    }
  }
}
</script>
.c-container {
width: 80%;
margin-right: auto;
margin-left: auto;
}
<style scoped>

</style>
