# Charter for Working Group

Domain Keys Identified Mail (DKIM, RFC 6376) defines a method for
using a digital signature to associate a domain identity with an email
message using an appropriate cryptographic authentication mechanism, and
to assure receiving domains that the message has not been altered since the
signature was created. Receiving systems can use this information as
part of their message-handling decision. This can help reduce spam,
phishing, and other unwanted or malicious email.

A DKIM-signed message can be re-posted, to additional recipients, in a
fashion that retains the original signature. With an author and a recipient
collaborating, this can "replay" the message, using the original signer's
reputation to propagate email with problematic content -- spam, phishing,
and the like.

Generally, the technical characteristics of this form of abuse match those of
legitimate mail, making its detection or prevention challenging. Timestamps
and carefully-tailored message signing conventions are appealing approaches
to replay mitigation. Each has significant limitations.

The DKIM working group will first develop and publish a clear problem statement.
Then, it will produce one or more technical specifications that propose
replay-resistant mechanisms. The working group will prefer solutions compatible
with DKIM's broad deployment, and there will be an expectation that these solutions
will have been through implementation and interoperability testing before publication.

If the working group decides that is unable to identify a consensus technical solution
to this problem space, it may instead publish a report describing the problem and
summarizing the reasons that none of the proposed approaches are acceptable.

Finally, the working group may produce documents that update operational advice to reflect
modern considerations, especially with respect to the replay problem described above.
This should be done only if there is a consensus opinion that such advice would be based
on experience rather than theory.

Current proposals include the following drafts:

 - draft-bradshaw-envelope-validation-extension-dkim
 - draft-chuang-dkim-replay-problem
 - draft-chuang-replay-resistant-arc
 - draft-gondwana-email-mailpath
 - draft-kucherawy-dkim-anti-replay

The working group may adopt or ignore these as it sees fit, and may consider or develop other proposals.

## Milestones

Date    Milestone   Associated documents

Dec 2023    Submit revised operational advice for replay-resistant DKIM use to the IESG at Informational
Dec 2023    Submit technical specifications for replay-resistant DKIM enhancement(s) to the IESG at Proposed Standard
Jun 2023    Proposal regarding plans for remaining document(s) presented to the AD
Apr 2023    Post a consensus problem statement draft to the datatracker (may not go to the IESG)
