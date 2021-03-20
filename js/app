$(document).ready(function () {
	// Добавить плавную прокрутку до всех ссылок
	$("a").on('click', function (event) {

		// Убедись в этом что .hash имеет значение перед переопределением поведения по умолчанию
		if (this.hash !== "") {
			// Запретить поведение щелчка якоря по умолчанию
			event.preventDefault();

			// Хранить хэш
			var hash = this.hash;

			// Использование метода animate() jQuery для добавления плавной прокрутки страницы
			// Необязательное число (800) указывает количество миллисекунд, необходимых для прокрутки до указанной области
			$('html, body').animate({
				scrollTop: $(hash).offset().top
			}, 900, function () {

				// Добавить хэш (#) для URL-адреса после завершения прокрутки (поведение щелчка по умолчанию)
				window.location.hash = hash;
			});
		} // Конец, если
	});
});
$(document).ready(function () {
	let btnSc = document.getElementById('top-btn')

	function HiddeScrollbtn() {
		if (window.pageYOffset > 300) {
			btnSc.style.opacity = '1'
		} else {
			btnSc.style.opacity = '0'
		}
	};
	window.onscroll = HiddeScrollbtn

	btnSc.onclick = function () {
		window.scrollTo({
			top: 20,
			behavior: "smooth"
		});
	}
	window.onscroll = HiddeScrollbtn
})
