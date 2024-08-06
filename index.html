let selectedProfessor = '';
let selectedDepartment = '';
let selectedUniversity = '';
let rating = 0;

// Example data for professors and reviews
const professors = {
    "Professor A": {
        department: "Computer Science",
        university: "University A",
        reviews: [
            { name: "John Doe", date: "2024-08-01", rating: 4, title: "Great Professor!", description: "Professor A is very knowledgeable and helpful." },
            { name: "Jane Smith", date: "2024-07-30", rating: 5, title: "Excellent Teaching", description: "The lectures are clear and concise." }
        ]
    },
    "Professor B": {
        department: "Mathematics",
        university: "University B",
        reviews: [
            { name: "Alice Johnson", date: "2024-07-28", rating: 3, title: "Average", description: "Decent professor, but could improve in explaining complex topics." }
        ]
    },
    "Professor C": {
        department: "Physics",
        university: "University C",
        reviews: [
            { name: "Bob Brown", date: "2024-08-01", rating: 5, title: "Fantastic!", description: "Professor C makes learning physics fun and engaging." }
        ]
    }
};

function filterProfessors() {
    const searchInput = document.getElementById('professorSearch').value.toLowerCase();
    const professorsList = document.querySelectorAll('#professorList li');
    professorsList.forEach(professor => {
        if (professor.textContent.toLowerCase().includes(searchInput)) {
            professor.style.display = '';
        } else {
            professor.style.display = 'none';
        }
    });
}

function viewProfessorDetail(name) {
    const professor = professors[name];
    selectedProfessor = name;
    selectedDepartment = professor.department;
    selectedUniversity = professor.university;
    document.getElementById('professorName').textContent = name;
    document.getElementById('professorDepartment').textContent = professor.department;
    document.getElementById('professorUniversity').textContent = professor.university;
    document.getElementById('professorDetail').style.display = 'block';

    // Load existing reviews
    const reviewsList = document.getElementById('reviewsList');
    reviewsList.innerHTML = '';
    professor.reviews.forEach(review => {
        const reviewElement = document.createElement('div');
        reviewElement.className = 'review';
        reviewElement.innerHTML = `
            <p><strong>${review.name}</strong> (${review.date})</p>
            <p>Rating: ${'&#9733;'.repeat(review.rating)}${'&#9734;'.repeat(5 - review.rating)}</p>
            <p><strong>${review.title}</strong></p>
            <p>${review.description}</p>
        `;
        reviewsList.appendChild(reviewElement);
    });
}

function closeModal() {
    document.getElementById('professorDetail').style.display = 'none';
}

function openReviewForm() {
    document.getElementById('reviewProfessorName').textContent = selectedProfessor;
    document.getElementById('reviewForm').style.display = 'block';
}

function closeReviewForm() {
    document.getElementById('reviewForm').style.display = 'none';
}

function rateProfessor(stars) {
    rating = stars;
    const starsElements = document.querySelectorAll('.rating span');
    starsElements.forEach((star, index) => {
        if (index < stars) {
            star.style.color = 'gold';
        } else {
            star.style.color = '';
        }
    });
}

function submitReview() {
    const reviewTitle = document.getElementById('reviewTitle').value;
    const reviewDescription = document.getElementById('reviewDescription').value;
    if (selectedProfessor && reviewTitle && reviewDescription && rating) {
        const review = {
            name: 'Anonymous', // You can modify this to capture the actual reviewer's name
            date: new Date().toISOString().split('T')[0],
            rating: rating,
            title: reviewTitle,
            description: reviewDescription
        };
        professors[selectedProfessor].reviews.push(review);
        alert(`Review submitted for ${selectedProfessor} with rating ${rating} stars:\nTitle: ${reviewTitle}\nDescription: ${reviewDescription}`);
        closeReviewForm();
        viewProfessorDetail(selectedProfessor); // Refresh the professor details to show the new review
    } else {
        alert('Please fill out all fields and rate the professor before submitting.');
    }
}
