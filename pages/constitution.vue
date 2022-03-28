<template>
  <Page title="Massachusetts Constitution">
    <img
      src="data:image/jpeg;base64,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"
    />
    <p>
      Massachusetts has a very similar constitution to the US government, but
      there are some differences that make it unique.
    </p>
    <ul>
      <li>
        <blockquote>
          The people of this commonwealth have the sole and exclusive right of
          governing themselves, as a free, soverign, and independant state; and
          do, and forever hereafter shall, exercise and enjoy every power,
          jurisdiction, and right which is not, or may not hereafter, be by them
          expressly delegated to the USA in congress Assembled.
        </blockquote>
        This is like a similar section of the US constitution. It provides
        protections to the people. Massachusetts gives the right to a direct
        democracy while US is republican.
      </li>
      <li>
        <blockquote>
          We, therefore, the people of Massachusetts, acknowledging, with
          grateful hearts, the goodness of the great Legislator of the universe,
          in affording us, in the course of His providence, an opportunity,
          deliberately and peaceably, without fraud, violence or surprise, of
          entering into an original, explicit, and solemn compact with each
          other; and of forming a new constitution of civil government, for
          ourselves and posterity; and devoutly imploring His direction in so
          interesting a design, do agree upon, ordain and establish the
          following Declaration of Rights, and Frame of Government, as the
          Constitution of the Commonwealth of Massachusetts.
        </blockquote>
        This is the preamble of the Massachusetts constitution. The main
        difference is that the Massachusetts constitution is much more
        religious. They are both similar types of government and define the name
        of the territory.
      </li>
      <li>
        <blockquote>
          In order to prevent those, who are vested with authority, from
          becoming oppressors, the people have a right, at such periods and in
          such manner as they shall establish by their frame of government, to
          cause their public officers to return to private life; and to fill up
          vacant places by certain and regular elections and appointments.
        </blockquote>
        This provides a system for impeachment. They both explain how the person
        is impeached. The difference with the MA constitiution is that the
        people impeach, not Congress.
      </li>
      <li>
        <blockquote>
          Any vacancy in the senate shall be filled by election by the people of
          the unrepresented district, upon the order of a majority of senators
          elected.
        </blockquote>
        They both provide a way for replacing senators, but Massachusetts has
        the people pick while the US has the governor pick.
      </li>
    </ul>
  </Page>
</template>
