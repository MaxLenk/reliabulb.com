---
layout: page
title: Contact
permalink: contact

---
<script src="https://www.google.com/recaptcha/enterprise.js?render=6Lei8nAkAAAAABwUbDWJpapl8dXb4OL9cYvE3qKd"></script>
<script>
    function formSubmit(e) {
        e.preventDefault();
        grecaptcha.enterprise.ready(async () => {
            const token = await grecaptcha.enterprise.execute('6Lei8nAkAAAAABwUbDWJpapl8dXb4OL9cYvE3qKd', {action: 'submit'});
            fetch('https://recaptchaenterprise.googleapis.com/v1/projects/reliabulb-1676161638722/assessments?key=AIzaSyDWC5lkvsrPkR43KyH-axzQkT3SeA_SBKI', {
                method: 'POST',
                headers: {
                    'Accept': 'application/json',
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify(
                    {
                        "event": 
                            {
                                "token": token,
                                "siteKey": "6Lei8nAkAAAAABwUbDWJpapl8dXb4OL9cYvE3qKd",
                                "expectedAction": 'submit'
                            }
                    })
            })
            .then(response => response.json())
            .then(response => {
                if (!response.hasOwnProperty("riskAnalysis")){
                    toggleModal("failure_modal");
                    return false;
                } else if (response.riskAnalysis.score > 0.5){
                    document.getElementById("contact_form").submit();
                    document.getElementById("contact_form").reset(); 
                    toggleModal("success_modal");
                } else{
                    toggleModal("failure_modal");
                    return false;
                }
            });
        });
    }
    function toggleModal(modalID){
        document.getElementById(modalID).classList.toggle("hidden");
        document.getElementById(modalID + "-backdrop").classList.toggle("hidden");
        document.getElementById(modalID).classList.toggle("flex");
        document.getElementById(modalID + "-backdrop").classList.toggle("flex");
    }
    document.addEventListener("DOMContentLoaded", function(){
        const params = new Proxy(new URLSearchParams(window.location.search), {
            get: (searchParams, prop) => searchParams.get(prop),
        });
        document.getElementById("subject").value = params.subject;
    });
</script>

<div class="font-sans mx-auto max-w-prose px-4 pt-4 prose-{{site.theme-color}}">
    <div class="g:py-16 px-4 mx-auto max-w-screen-md">
        <p class="font-light text-center text-gray-600 text-xl">
            Power supply design, LED lighting, expert witness, and more. Contact me here to see how I can help you.
        </p>
        <div class="grid place-content-center py-8">
            <a href="{{site.linkedin}}" target="_blank" class="no-underline">
                <div class="relative border border-black overflow-hidden rounded-full grid place-content-center prose transition-all
                duration-500 bg-gradient-to-tl from-blue-300 via-gray-300 to-gray-300 bg-size-200 bg-pos-0 hover:bg-pos-100">
                    <div class="text-base font-bold p-4">Or contact me on LinkedIn.</div>
                </div>
            </a>
        </div>
        <form action="https://api.web3forms.com/submit" method="POST" id="contact_form" class="space-y-8" onsubmit="return formSubmit(event)" target="hiddenFrame">
            <input type="hidden" name="access_key" value="da4dc033-c216-47fd-a1f1-827d22411c04">
            <input type="checkbox" name="botcheck" class="hidden" style="display: none;">
            <div>
                <label for="email" class="block mb-2 text-sm font-medium text-gray-600">Your Email</label>
                <input type="email" name="email" class="shadow-sm bg-yellow-200 border border-black text-gray-900 text-sm rounded-lg focus:ring-black block w-full p-2.5 placeholder-gray-500" placeholder="name@address.ext" required>
            </div>
            <div>
                <label for="subject" class="block mb-2 text-sm font-medium text-gray-600">Subject</label>
                <input type="subject" name="subject" id="subject" class="shadow-sm bg-yellow-200 border border-black text-gray-900 text-sm rounded-lg focus:ring-black block w-full p-2.5 placeholder-gray-500" placeholder="What can I help you with?" required>
            </div>
            <div class="sm:col-span-2">
                <label for="message" class="block mb-2 text-sm font-medium text-gray-600">Message</label>
                <textarea name="message" rows="6" class="block p-2.5 w-full text-sm text-gray-900 bg-yellow-200 rounded-lg shadow-sm border border-black focus:ring-black placeholder-gray-500" placeholder="Details of your request."></textarea>
            </div>
            <div class="flex flex-col items-center pb-16">
                <button type="submit" class="g-recaptcha py-3 px-5 text-md font-medium text-center text-gray-600 rounded-full border border-black transition-all duration-500 bg-gradient-to-tl from-yellow-200 via-white to-white bg-size-200 bg-pos-0 hover:bg-pos-100 focus:transition-none focus:border-gray-900">
                        Submit
                </button>
            </div>
        </form>
        <iframe name="hiddenFrame" width="0" height="0" border="0" style="display: none;"></iframe>
    </div>
</div>


<div class="hidden overflow-x-hidden overflow-y-auto fixed inset-0 z-50 outline-none focus:outline-none justify-center items-center" id="failure_modal">
  <div class="relative w-auto my-6 mx-auto max-w-3xl">
    <!--content-->
    <div class="px-8 pt-8 border-0 rounded-lg shadow-lg relative flex flex-col w-full bg-white outline-none focus:outline-none">
      <!--header-->
        <p class="text-3xl font-semibold text-center">
            Error - The form confused you with a robot.
        </p>
      <!--body-->
      <div class="relative p-6 flex-auto">
        <p class="text-md text-black max-w-prose text-center">
          Please contact me through my <a href="{{site.linkedin}}" class="underline" target="_blank">LinkedIn profile</a>.
        </p>
      </div>
      <!--footer-->
      <div class="flex flex-col items-center py-8">
        <button class="g-recaptcha py-3 px-5 text-lg font-medium text-center text-black rounded-full border border-transparent transition-all duration-500 bg-gradient-to-tl from-yellow-200 via-white to-white bg-size-200 bg-pos-0 hover:bg-pos-100 focus:transition-none focus:border-gray-900" type="button" onclick="toggleModal('failure_modal')">
          Close
        </button>
      </div>
    </div>
  </div>
</div>
<div class="hidden opacity-25 fixed inset-0 z-40 bg-black" id="failure_modal-backdrop"></div>

<div class="hidden overflow-x-hidden overflow-y-auto fixed inset-0 z-50 outline-none focus:outline-none justify-center items-center" id="success_modal">
  <div class="relative w-auto my-6 mx-auto max-w-3xl">
    <!--content-->
    <div class="px-8 pt-8 border-0 rounded-lg shadow-lg relative flex flex-col w-full bg-white outline-none focus:outline-none">
      <!--header-->
        <p class="text-3xl font-semibold text-center">
            Success - Thank you for contacting me.
        </p>
      <!--body-->
      <div class="relative p-6 flex-auto">
        <p class="text-md text-black max-w-prose text-center">
          I will get back to you soon. Check out my <a href="{{site.linkedin}}" target="_blank">LinkedIn profile</a>.
        </p>
      </div>
      <!--footer-->
      <div class="flex flex-col items-center py-8">
        <button class="g-recaptcha py-3 px-5 text-lg font-medium text-center text-black rounded-full border border-transparent transition-all duration-500 bg-gradient-to-tl from-yellow-200 via-white to-white bg-size-200 bg-pos-0 hover:bg-pos-100 focus:transition-none focus:border-gray-900" type="button" onclick="toggleModal('success_modal')">
          Close
        </button>
      </div>
    </div>
  </div>
</div>
<div class="hidden opacity-25 fixed inset-0 z-40 bg-black" id="success_modal-backdrop"></div>