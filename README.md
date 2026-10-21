console.log("Welcome to Skill Swap!");

const detailButtons = document.querySelectorAll(".details-button");

detailButtons.forEach(function (button) {
    button.addEventListener("click", function () {
        const card = button.closest(".skill-card");
        const details = card.querySelector(".extra-details");

        details.hidden = !details.hidden;

        button.textContent = details.hidden
            ? "Show Details"
            : "Hide Details";
    });
});
