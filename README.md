# AirlineFeedback
A Streamlit app for a fictional airline that collects passenger ratings and comments, uses a Groq-powered LLM to categorize feedback, and provides an owner dashboard to identify improvement priorities and flag comments for manual review.

## Business Question

Which part of the passenger experience should Skyline Air
prioritize improving?

## Labels

- **Flight Delays:** Feedback about delays, cancellations,
  or missed connections.
- **Staff & Service:** Feedback about flight attendants,
  gate agents, check-in, or customer support.
- **Seating & Comfort:** Feedback about seats, legroom,
  cabin cleanliness, temperature, or onboard amenities.
- **Baggage:** Feedback about lost, delayed, damaged,
  or mishandled luggage.
- **Price & Value:** Feedback mainly about fares, extra fees,
  refunds, or overall value.
- **Manual Review:** Feedback that is unclear, unrelated,
  too general, or has no clear main topic.

Each written comment receives exactly one label.
Rating-only submissions are saved without a label.

## Customer Side

Customers can submit a star rating, a written comment, or both.
At least one is required.

## Owner Side

The password-protected dashboard shows:
- Total submissions
- Average star rating
- Number of comments needing manual review
- Low-rated comment counts by category
- Average ratings by category
- Full comments needing manual review

## Limitations

LLM labels can be incorrect. Unclear comments and API failures
are routed to manual review.

This course demo stores feedback in SQLite. Local storage on
Streamlit Community Cloud is not guaranteed to persist.
A hosted database would be needed for lasting collection.

Skyline Air is fictional. This is a student project.
