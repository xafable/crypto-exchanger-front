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



              This Privacy Policy (hereinafter referred to as the Policy) defines the policy regarding the processing of personal data, contains information on the implemented requirements for the protection of the Operator's personal data.
              1. Terms and definitions

              1.1. Data subject - an individual who has reached the age of majority using the Site on the Internet unlimited.com for financial transactions with electronic, digital or fiat currency.

              1.2. Cookies - a piece of data as part of an HTTPS request, intended for storage on the Subject's end device and used by the Operator to identify the Subject.

              1.3. Site - a set of programs for electronic computers and other information in the information and telecommunications network "Internet", designed to be displayed in a browser and accessed using the domain name of the Operator. In the context of the Operator's activities, the site unlimited.com is used

              1.4. Registration data - a list of information specified by the Operator when registering on the unlimited.com website, and later when they change during the execution of the contract.

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

              2.5. This Policy is published on the Internet on the website unlimited.com.
              3. Categories of personal data subjects

              3.1. The Operator processes the personal data of all Data Subjects who are Users of the unlimited.com website.
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

              Effective date: 01.05.22.

            </p>
          </q-tab-panel>

          <q-tab-panel name="terms">
            <div class="text-h4 q-mb-md">Terms of use</div>
            <p>


              This agreement is located for public access on the Internet on the page unlimited.com and can be changed by the Service Manual unilaterally without additional notice to the User.

              The parties to this agreement are unlimited.com, hereinafter simply the "Service" and any individual using the services of the Service, hereinafter referred to as the "User".
              1. Terms and definitions

              1.1. unlimited.com is a trademark that is the name for a cryptocurrency exchange point and offers its services through a special software interface for all Users.

              1.2. A user is any natural person using the services of the unlimited.com service.

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
            <p>
              This agreement describes the conditions on the basis of which the services of the "unlimited.com" service are provided. Before using the services of the service, the User is obliged to read and accept all the terms of this agreement. Otherwise, the User cannot use the services of the service.

              This agreement is located for public access on the Internet on the page unlimited.com and can be changed by the Service Manual unilaterally without additional notice to the User.

              The parties to this agreement are "unlimited.com", hereinafter simply "Service" and any individual using the services of the Service, hereinafter referred to as "User".

              1. Terms and definitions
              1.1. "unlimited.com" is a trademark that is the name for an electronic currency exchange office and offers its services using a special software interface for all Users.

              1.2. A user is any individual using the services of the unlimited.com service.

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

              - to exclude in their practical activities using the Service any actions, providing the existence of which may cause direct or indirect harm to the fight against money laundering and legalization of illegally obtained funds;

              3.9. The Service undertakes to take all possible and available actions to prevent attempts of illegal trade, financial fraud and money laundering using the services of the Service. These actions include but are not limited to:

              - provide all possible assistance to law enforcement agencies in the search and capture of financial terrorists engaged in illegal activities of money laundering.

              - providing the competent authorities, in accordance with applicable law, with information regarding the processing of the Service;

              - improving the Service to prevent direct or indirect use of the Service in activities that are contrary to legislation aimed at combating illegal trade, financial fraud and money laundering.

              4. Service services
              4.1. Ordering the services of the Service and obtaining information about the progress of the transaction by the User are made exclusively through contacts with a representative of the Service.

              4.2. The service offers its services without a break for lunch and will strive to ensure that services are provided seven days a week and around the clock.

              5. Cost of services
              5.1. Tariffs are determined by the management of the Service and published on the website of the Service. The Administration of the Service has the right to change the tariffs of the Service without additional notice.

              5.2. In addition to the established rates, the User also reimburses all additional costs for postage, telephone, fax, etc., incurred in the course of business relations with the Service.

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

              8.8. The user undertakes not to falsify communication flows, which are related to the operation of the Service.

              8.9. The User acknowledges that the content of the Service website is protected by the laws on the protection of property rights, intellectual property and copyrights. Unauthorized use of this content is illegal.

              9. Force majeure
              9.1. Neither the User nor the Service will be liable to each other for delays or failure to fulfill their obligations resulting from the occurrence of force majeure circumstances, including natural disasters, fire, flood, terrorist attacks, power shifts, civil unrest, as well as non-functioning of Payment systems, energy supply systems , communication networks and Internet service providers.
            </p>

          </q-tab-panel>


        <q-tab-panel name="regulations">
          <div class="text-h4 q-mb-md">Regulations</div>
          <p>
            User agreement with the exchange resource

            1. GENERAL PROVISIONS
            1.1. This Agreement defines the conditions for the provision of services by the exchange platform.

            1.2. The exchange platform refers to the unlimited.com web resource, the functions of which include the exchange of electronic and digital monetary units.

            1.3. Clients are individual citizens and enterprises that have expressed their intention to carry out an exchange operation through an exchange platform (hereinafter referred to as the Platform).

            1.3.1 The Client warrants that he is not a citizen of the United States, Iran, North Korea or China, is not acting on behalf of a company whose ultimate beneficiary is a citizen of the United States, Iran or China, and is not on the sanctions list of any state.

            1.4 When jointly referring to the Platform and the Client, they are referred to as the Parties.

            1.5 The Parties have agreed that this electronic Agreement has the force of a written agreement.

            1.6. This Agreement is a public offer accepted through the execution of an exchange application on the unlimited.com web resource.

            2. SUBJECT OF THE AGREEMENT
            2.1. The services provided by the Platform are given in clause 4. The procedure for their provision is provided for by the Regulations, the procedure of which is described in clause 5. The Client is obliged to comply with the conditions of clause 9.

            2.2. Exchange services are paid. The client who made the exchange through the Platform must pay the appropriate fee.

            3. The platform has the right
            3.1. Suspend activities for technical work, as well as troubleshooting.

            3.2. Stop the conversion if the Client complained about fraud, partners asked about it or employees of the competent authorities demanded it.

            3.3. Independently set the amount and procedure for granting discounts.

            3.4. Approve and change the amount of commissions for performing operations.

            3.5. Deny service without explanation.

            3.6. If an error was made during the operation, the Platform administration has the right to demand its confirmation and confirmation of involvement in the operation using E-mail or screenshots.

            3.7. Terminate the dialogue with the Client who demonstrates inappropriate behavior, or if he refuses to provide the information necessary to complete the application.

            3.8. Block the transfer in the event of a situation described in clauses 5.4.-5.6.

            3.9. In case of unjust enrichment by the Client with electronic money of the unlimited.com web resource, or third-party services for the exchange of electronic money, the site administration has the right to suspend the execution of the application until the reasons and all circumstances are clarified, as well as compensation for losses incurred by the Platform or other exchange services .

            3.10. In case of payment later than the set time, as well as in case of confirmation of the transaction for more than 5 minutes due to sending funds with a commission below the recommended one, the service has the right to recalculate the exchange rate.

            4. Platform commits
            4.1. Convert, under the conditions described by the Regulations, EPS title units, or fiat funds from bank cards from which payment is made.

            4.2. Provide the Client with access to information regarding the working conditions of the Platform, as well as technical support for exchange operations via email support@unlimited.com

            4.3. Guarantee the confidentiality of transaction data, including their amount and execution time. The relevant data is available only to the Client who made the transfer.

            4.4. Limit the access of unauthorized persons to information about the conversion, with the exception of situations requiring external arbitration, in the event that the platform is accused of dishonest performance of duties by the client.

            5. LIST OF SERVICES PROVIDED
            5.1. The platform carries out exchange operations with the participation of electronic monetary units.

            5.2. Among the Partners are banks according to the specified list.

            5.3. The Platform does not have the authority to verify the legality of the Client's possession of the assets used in the course of the exchange operation.

            6. FORCE MAJOR
            6.1. In the event of force majeure events, the Parties shall not be liable for non-fulfillment or improper fulfillment of contractual obligations. Unforeseen circumstances include a terrorist act, military conflict, fire, cyber attack, flood, other natural disasters, the decision of the authorities, as well as lack of access to energy, failure or failure of the site system or blockchain operation, telecommunications networks, the Internet.

            6.2. In case of blocking a transaction or an account by a bank or EPS, the parties act by analogy with Clause 3.2.4. and 5.5 respectively.

            7. EXCHANGE PROCEDURE
            7.1. The Client is not entitled to use the functionality of the Platform to make illegal transactions. The Client is aware that he will be held liable for the conversion of doubtful funds. Responsibility arises according to the norms of the state in whose jurisdiction the violation took place.

            7.2. If there has been a conversion of doubtful funds, the Platform reserves the right to inform the injured party, law enforcement agencies or EPS about this, at their request.

            7.3. To make an exchange, the Client must transfer from the electronic wallet the required amount of the corresponding monetary units. Platform employees have no grounds to verify the legality of their use, but not the origin. The client warrants that he has the legal authority to use the money in the conversion process.

            7.4. A bank transfer involves the use of an Internet banking system and EPS to ensure payment security.

            7.5. The Platform is not responsible for the exchange operation performed by third parties with the consent of the Client.

            7.6. If the Client activates the option "I agree with the exchange rules", then he expresses full acceptance of all the terms of this Agreement.
          </p>
        </q-tab-panel>

        <q-tab-panel name="rules">
          <div class="text-h4 q-mb-md">Rules</div>
          <p>
            Date of entry into force: 01.05.22.

            Disclaimer:
            unlimited.com hereby notifies the Users of the unlimited.com website that the possession of digital financial assets, as well as the implementation of operations with digital financial assets, is accompanied by the risk of losing personal financial resources. The value of digital currencies may increase or decrease, which may entail the risk that you will lose your funds by buying, selling, holding or investing them in digital assets.

            Trading virtual assets and digital assets also involves special risks that are not usually associated with official currencies. Unlike most currencies that are backed by governments or other entities, or commodities such as gold or silver, virtual assets are a unique kind of fiat currency backed by technology and trust. There is currently no government agency that can issue more virtual currency or take corrective action to protect the value of virtual assets in times of crisis.

            When working with digital financial assets, there may be other risks that are not provided for by this User Agreement and the Administration of the unlimited.com website.

            General provisions
            This user agreement (hereinafter referred to as the Agreement, the User Agreement) governs the relationship between unlimited.com and Users of the unlimited.com website, who are residents and non-residents of the CIS countries.

            By using the unlimited.com website (Site), by registering an account (Account) to use the unlimited.com service, you agree that you have read, understood and accepted all the terms and conditions contained in this Agreement, as well as in the Policy privacy.

            In addition to the terms of this user agreement, the User is obliged to read the statement confirming the legality of the origin of funds and/or cryptocurrency assets.

            If you do not agree with the terms of the User Agreement, the use of the unlimited.com website is not allowed.

            1. Eligibility
            1.1. You hereby agree and acknowledge that you: are of legal age to accept these terms; you have not been previously suspended or prohibited from using the Services.

            1.2. If you are using the Services on behalf of a legal entity, you also represent and warrant that: the legal entity is properly registered and operating in accordance with the applicable laws of its jurisdiction of incorporation, and such legal entity has authorized you to act on its behalf.

            2. Terms and definition
            2.1. unlimited.com is a trademark of a system that provides Users with the opportunity to exchange digital and electronic currencies.

            2.2. Service - a system for providing Internet services for the exchange, sale and purchase of digital and / or electronic currencies.

            2.3. A user is any natural person using the services of the unlimited.com service.

            2.4. Digital currency - Bitcoin, Litecoin, Ethereum and any other blockchain-based currencies.

            2.5. E-currency - funds held on the accounts of users of electronic payment systems (Payoneer, PayPal etc.).

            2.6. A payment system is a software and hardware product developed by a third party and is a mechanism for implementing the accounting of monetary obligations, as well as organizing mutual settlements between its users.

            2.7. Service Services - assistance in conducting p2p transactions between individuals for the purchase and sale and exchange of digital currencies, as well as other services, information about which is posted on the Service window.

            2.8. Payment is a transfer of digital currency or fiat funds from the User to the User or the Service, as well as in the opposite direction.

            2.9. Application - an expression of the User's intention to use one of the services offered by the Service by filling out an electronic form through the Service's website, on the terms described in the Agreement and specified in the parameters of this Application.

            2.10. Partner - a person who provides the Service with services to attract Users, the terms of which are described in this Agreement.

            2.11. Rate — the cost ratio of two digital currencies during their exchange.

            2.12. "Messages" includes email messages.

            3. Rules for using an account on the site unlimited.com
            3.1. The unlimited.com website is intended for personal use only. By registering on the site, you consent to the transfer of reliable data about yourself to unlimited.com in accordance with the registration procedure on the Site. You also agree that you will not use any account other than your own, nor will you attempt to gain unauthorized access to the accounts of other users. In addition, the User agrees that he can have only one account on the unlimited.com website.

            3.2. We can also carry out additional valid verification of your information and request from you any necessary documentation and data related to the exchange (passport, card photo, video verification of the card, receipt of sending funds and other necessary data) for any reason related to your use of the services and / or as supporting evidence for any information you provide. If the conditions for providing documents are not met, the service has the right to refuse to provide services and initiate a refund to the sender's details within 5 banking days, minus the commission within the payment system network.

            3.2.1 The unlimited.com Service has the right to block the User's operation, in order to prevent fraudulent and other actions that may cause financial and reputational losses for the Service or the User, for the period required to conduct a financial investigation and obtain details of the transaction from the payment gateway or issuing bank.

            3.3. The Administration of the unlimited.com website may, at any time and in its sole discretion, deny you the opportunity to open an Account, limit the Account or suspend any transaction until the end of consideration of any information provided by you.

            3.4. Your account privacy. You acknowledge that you are responsible for maintaining the strict confidentiality of your Account information, including your password, protecting your own Digital Currency, and for all activities and transactions posted to your Account. You understand that any compromise of your login information may expose your Account to unauthorized access by third parties, which may result in the loss or theft of Digital Currency or funds from your Account, including linked accounts such as linked bank accounts and credit cards.

            3.5. Security Alerts. In order to receive security notices from the Company, you must notify the Company of changes to your email address and telephone number. Under no circumstances will the Company be liable for any direct damages or losses that you may suffer as a result of compromised account login credentials due to no fault of the Company and/or failure to follow or act on any notices or warnings about that we can send to you. Notwithstanding the foregoing, the Company does not guarantee or take any other action in relation to you, and shall not be liable for such warnings.

            3.6. You must notify us immediately of any unauthorized use of your Account or password, suspected breach of your login information, or any other breach of security by e-mail info unlimited.com.

            3.7. Responsibility for the actions of third parties. Your account is for personal use only and not for use or access by any third party. In any case, you are solely responsible for all acts or omissions of any third party accessing and/or using your Account.

            3.8. You agree that you will not use the Services to engage in any criminal activity, including but not limited to the purchase of prohibited substances, money laundering, illegal gambling, terrorist financing. You warrant that you will strictly adhere to the AML policy of the service.

            In addition, you warrant that you will not use methods to obscure the location from which you access the Site and that you will disclose to the Company, upon request, your exact and true location. If the Company, based on the analysis of user transactions, or using special technical means, determines that the activity on your Account is suspicious or related to any prohibited activity or illegal operation, the Company may suspend your Account, block any outstanding transactions, reject any subsequent transactions.

            Blocked exchange transactions will be returned to the sender's details within 3 working days, minus a 5% service fee, to cover the total cost of labor costs for processing the application and arranging a refund.

            4. Services provided on the site unlimited.com
            4.1. The Service allows the User to register an account free of charge. However, the Service charges a fee for the services provided. The size of the commission is determined by the Site Administration unilaterally and may change.

            The service is obliged to provide up-to-date information regarding the commission for services in the rules of the site. Ordering the services of the unlimited.com. Service is carried out by the User by sending the corresponding Application through the website on the Internet with the domain name unlimited.com.

            4.2. By using the service

            ca, the User confirms that he legally owns and disposes of the fiat money and electronic and/or digital currency involved in the relevant Payment.

            4.3. The unlimited.com service provides the following services:

            A service to provide the User with the opportunity to sell electronic and / or digital or fiat currency to another User in real time.

            A service to provide the User with the opportunity to buy electronic and / or digital or fiat currency from another User in real time.

            4.4. By filling out the Application, the User instructs, and the Service, on its own behalf and at the expense of the User, performs actions to sell and transfer digital and / or electronic or fiat currency to another User.

            4.5. The amount of remuneration of the Service for the specified actions in the amount of 1% of the transaction amount. The reward is taken into account and confirmed in the Application by the User on one of the pages of the user interface.

            4.6. Within the time allotted by the regulations (depending on the direction of the exchange) from the moment of receipt of funds from the User, in the amount specified in the relevant Application, the Service is obliged to transfer (transfer) the Received electronic or fiat currency to the details and in the amount specified by the User in the Application, if this is not prevented by force majeure circumstances.

            4.7. The Service has the right to cancel an application created by the User for the purchase of digital and / or electronic or fiat currency, if payment for such an application has not been received on the service’s settlement account after 30 (thirty) minutes from the moment such an application was created.

            4.8. The obligation of the Service to transfer (transfer) the Received digital and / or electronic or fiat currency to the User is considered fulfilled at the moment the digital and / or electronic or fiat currency in the relevant Payment system is debited from the account of the Service, which is recorded in the transaction history of the corresponding Payment system.

            4.9. By filling out the Application, the User instructs, and the Service, on its own behalf and at the expense of the User, buys electronic and / or digital or fiat currency from another User, and also performs actions to transfer the monetary equivalent to the User in the amount specified in the Application.

            4.10. Within the time allotted by the regulations (depending on the direction of exchange) from the moment of receipt of electronic and / or digital or fiat currency from the User, in the amount specified in the relevant Application, the Service is obliged to transfer to the User the monetary equivalent of the transferred digital and / or electronic or fiat currency, by the method selected by the User when creating the Application.

            4.11. The obligation of the Service to transfer the monetary equivalent of the transferred digital and / or electronic or fiat currency is considered fulfilled at the time the corresponding amount is debited from the account of the Service.

            4.12. All services of the unlimited.com service are provided without any express or implied warranties, in particular, without the implied warranties of merchantability and fitness for a particular purpose. The Company does not guarantee that the unlimited.com services, as well as the unlimited.com website, will be available in 100% of cases to meet your needs. The Company will strive to provide you with its services as soon as possible, but there is no guarantee that access will not be interrupted or that there will be no delays, failures, errors, omissions or loss of transmitted information.

            4.13. unlimited.com will make reasonable efforts to provide access to the services and the unlimited.com website in accordance with this Agreement. However, unlimited.com may suspend your use of the site for maintenance purposes and will use reasonable efforts to notify you in advance. Thus, you agree that you assume the risks associated with the fact that you may not always be able to use the services and the site unlimited.com or perform urgent transactions using your account.

            Addition to the procedure for the provision of services:

            4.14. The rate is fixed when creating an application, if the User paid for it within 30 minutes after the creation. If payment is not received within 30 minutes, then the application is deleted automatically and, in order to restore the application, the User must contact the technical support of the site. In this case, the amount of payment on the application will be recalculated at the rate at the time of receipt of payment.

            4.16. If the User has paid for the application, but due to circumstances wishes to refuse the exchange, then the refund is made minus 3% of the payment amount, the commission within the payment system network and the exchange rate difference (if the exchange rate has changed by more than 3%)

            4.17. If the User has paid later than this time, the Service reserves the right not to execute and not to return the funds paid to the User.

            4.18. If the User transferred an incorrect amount of electronic assets according to created before application the Service has the right to cancel this transaction because of inability to define a transaction as a payment by the bot system. The User has the opportunity to restore the transaction by making an Duplicate Order. Duplicate Order is identical application and transaction in order to find the previous one and combine them for successfully pay out by the bot system. The exchange rates are rate fixed by the first application will be used for pay out. For its part, the Service undertakes to help the User perform a successful Duplicate Order. User also have an manual search option which includes stopping the service and further search by the employees of the Service for the transaction of the User for further payment.

            4.19. The application should be paid exclusively through the payment form on our website (merchant), which is available after clicking the "go to payment" button. Unauthorized payment by details is not allowed. Otherwise, the application may be cancelled.

            4.20. The provision of services to the User is carried out in accordance with the legal requirements in force in the jurisdiction in which such services are provided.

            5. Cost of services
            5.1. Tariffs are determined by the management of the Service and published on the website of the Service. The Administration of the Service has the right to change the tariffs of the Service without additional notice.

            6. Taxation
            6.1. The Service is not a tax agent for the User and will not notify the User of his tax costs. The User undertakes to independently pay all taxes required in accordance with the tax laws of his jurisdiction.

            6.2. In the event that the authorities require the Service to pay the User's taxes or cover the debt resulting from the User's refusal to pay taxes, the User agrees to reimburse the Service for all these payments.

            7. Guarantees and liability of the parties
            7.1. The unlimited.com Service is financially liable to the User in the amount of the electronic asset or electronic money that was transferred to the unlimited.com Service for the execution of the Application.

            7.2. The unlimited.com service provides services for the exchange, purchase and sale of electronic assets. The unlimited.com service does not provide fundraising services, does not provide payment for goods or services of other providers.

            7.3. The unlimited.com service is not liable to the User for financial losses caused by illegal actions of third parties that cannot be predicted or prevented.

            7.4. The unlimited.com service is not responsible for any pending or unrealized Applications caused by an error of another Payment system or bank specified by the user in the completed Application. The user agrees that in this case all claims will be sent to the payment system or bank. The unlimited.com service will provide the necessary assistance to file a complaint or claim to another partner or bank.

            7.5. In case of detection of falsification of communication flows or any negative impact on the normal operation of the program code of the Service, which is directly or indirectly related to the User's Application, the execution of the Application by the Service is suspended, and according to the funds already received, the parameters of the Application are recalculated in accordance with the current conditions or, in case of disagreement of the User with the recalculation, return of the electronic asset or funds to the details of the payer.

            7.6. The unlimited.com service is not responsible for partial or complete non-compliance with these Terms of Use, if such was the result of force majeure circumstances that cannot be prevented by reasonable measures.

            7.7. In other cases, failure to fulfill obligations arising from these Terms or violation of certain terms will be considered in accordance with the laws of the country in whose jurisdiction the User is located.

            7. Responsibility of the User:

            7.8. The user is responsible for the accuracy and completeness of the information and data that he provided during registration. In the event that the User entered incorrect personal data or provided incorrect data for the execution of the Application, the unlimited.com Service is not responsible for any losses of the User resulting from such an error.

            7.9. In case of acceptance of these Terms, the User honestly declares and confirms that:

            7.10. He provided correct and truthful information about himself, as well as true identification data;

            7.11. He is not a participant in money laundering operations or transactions;

            7.12. His income is not related to the implementation of criminal and / or terrorist activities;

            7.13. His income is not related to the implementation of trade in countries in which trade is prohibited by international organizations;

            7.14. His income is not related to any other illegal activity.

            7.15. The User undertakes not to disrupt the operation of the unlimited.com Service by interfering with its software or hardware, as well as by distorting the parameters transmitted to the Service.

            7.16. The User acknowledges and agrees that The unlimited.com Service does not act as a financial advisor, does not provide investment advisory services, and any communication between the User and the unlimited.com Service cannot be considered as advice.

            7.17. The User is not responsible for partial or total non-compliance with these Terms and Conditions, if it is caused by the occurrence of force majeure, unforeseen events or prevented by appropriate measures.

            7.18. In other cases, failure to fulfill obligations arising from these Terms and Conditions or violation of individual Terms and Conditions will be considered in accordance with the laws of the country in whose jurisdiction the User is located.

            7.19. In the event that the client noticed a discrepancy with the broadcast of courses on monitoring. The client is obliged to notify the technical support of the service about this. For which, it can be rewarded with an increase in the level of the loyalty program.

            In the event that the client took advantage of a technical failure on the side of the unlimited.com exchange office and the exchange office incurs financial or reputational losses. These actions will be regarded as fraud. The client is subject to blocking, and all incomplete orders can be withheld to compensate for the loss of the service.

            8. Applicable law and jurisdiction
            8.1. This agreement, as well as all disputes related to it, shall be considered in accordance with the laws of the United Kingdom.

            9. Other terms
            9.1. The use of the unlimited.com Service for the purpose of carrying out fraudulent and illegal operations is prohibited.

            9.2. Operators of the unlimited.com service are legally required to provide information about payments, Users and Transactions to any government authorities that have the legal right to request relevant information.

            9.3. The protection of User information and other confidential data of citizens is ensured in accordance with the current legislation on the storage of personal data, in accordance with the jurisdiction of the User.

            9.4. The method of processing and protecting personal information is described in detail in the Privacy Policy published on the website of the unlimited.com. Service, which is required to conclude a contractual relationship between the User and the unlimited.com Service.

            9.5. Service unlimited.com in case of suspicious actions in the process of filling out an application by the User, in order to avoid damage from hacker attacks, has the right to suspend the execution of such operations until the reasons for these actions are clarified.

            9.6. The unlimited.com Service has the right to refuse to perform the operation of exchanging, buying and selling electronic currencies if the transfer of an electronic asset to the Service account was made without filling out an Application using the user interfaces on the Service Website. The electronic currency transferred to the relevant accounts of the Service by the User without filling out an Application using the user interfaces on the Service Website can be returned to the User upon request, taking into account the deduction of the payment system commission.

            9.7. The Service Administration has the full right to refuse to provide services to any User without explanation.

            9.8. Information about the User and his operations is stored on the server and cannot be deleted. At the request of the User, access to the account can be limited or deleted.

            9.9. The response time of the unlimited.com Service to the User's requests may be up to five business days from the date of receipt of the corresponding request from the User.

            10. Force majeure
            10.1. If, in the event of a force majeure event, you or unlimited.com are delayed or unable to comply with any of these Terms, then such delay or non-compliance will not be considered a violation of these Terms, and neither you nor the unlimited.com Service cannot claim any loss or damage resulting from such circumstances.

            11. Final provisions
            11.1. The terms and conditions are agreed with the User in electronic form during registration. The agreement with the Terms published in electronic form is valid and identical to the written consent.

            11.2. The unlimited.com Service has the right to unilaterally amend the Agreement by publishing the changes on the Service Website. The changes come into force from the moment of publication, unless another date for the entry into force of the changes is additionally determined when they are published. The User has the right to terminate the contractual relationship with the unlimited.com. Service due to his disagreement with the change in such Terms. The User must notify the unlimited.com. Service of his disagreement with the change in the Terms and termination of the contractual relationship by sending a corresponding letter to info@unlimited.com.

            11.3. The unlimited.com service has the right to send the User information on the status of the exchange process, as well as other information, including advertising, to the e-mail specified by him. The user can unsubscribe from advertising mailings by clicking on the appropriate button in the received letter.

            11.4. The information posted on the site, including all graphic images, textual information, program codes, etc., is the property of unlimited.com. and is protected by copyright laws.

            11.5. The User confirms that he is familiar with all the provisions of these Terms and fully accepts them.

            12. Contact details
            12.1. You can communicate with unlimited.com employees during business hours using the available messenger indicated on the unlimited.com website. You can also send an email to info support@unlimited.com.
          </p>
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
