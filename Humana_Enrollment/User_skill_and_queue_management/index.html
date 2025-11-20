<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>User Management</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f2f5;
        }
        .custom-checkbox:checked {
            background-image: url("data:image/svg+xml,%3csvg viewBox='0 0 16 16' fill='white' xmlns='http://www.w3.org/2000/svg'%3e%3cpath d='M12.207 4.793a1 1 0 010 1.414l-5 5a1 1 0 01-1.414 0l-2-2a1 1 0 011.414-1.414L6.5 9.086l4.293-4.293a1 1 0 011.414 0z'/%3e%3c/svg%3e");
            border-color: #2563eb;
            background-color: #2563eb;
        }
        .table-header {
            background-color: #f8fafc;
        }
        .table-row:hover {
            background-color: #f1f5f9;
        }
        .table-fixed {
            table-layout: fixed;
        }
        .pagination-button.active {
            background-color: #3b82f6;
            color: white;
            border-color: #3b82f6;
        }
        .tab-active {
            background-color: #65a30d;
            color: white;
            position: relative;
        }
        .tab-active::after {
            content: '';
            position: absolute;
            bottom: -8px;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 0;
            border-left: 8px solid transparent;
            border-right: 8px solid transparent;
            border-top: 8px solid #65a30d;
        }
        @keyframes pulse-glow {
            0%, 100% {
                color: #2563eb;
                text-shadow: 0 0 2px rgba(59, 130, 246, 0);
            }
            50% {
                color: #3b82f6;
                text-shadow: 0 0 8px rgba(59, 130, 246, 0.7);
            }
        }
        .pulse-glow {
            animation: pulse-glow 2.5s infinite;
        }
    </style>
</head>
<body class="p-4 sm:p-6 lg:p-8">

    <div class="max-w-7xl mx-auto">

        <!-- PAGE 1: User Profile View -->
        <div id="page-profile">
            <!-- Header Section -->
            <div class="mb-6">
                <div class="flex justify-between items-center mb-4">
                    <h1 id="user-header" class="text-4xl font-light text-gray-800"></h1>
                </div>
                <div class="flex items-center gap-4 border-b border-gray-200">
                    <button class="py-2 px-4 text-sm font-semibold rounded-t-md tab-active">Summary</button>
                    <button class="py-2 px-4 text-sm font-semibold text-gray-600 hover:text-gray-900">Audit Details</button>
                </div>
            </div>

            <!-- Main Content Area -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
                <!-- Center Column (Queues) -->
                <div class="lg:col-span-2 bg-white p-6 rounded-lg border border-gray-200 shadow-sm">
                    <div class="flex justify-between items-center mb-4">
                        <h2 class="text-xl font-semibold text-gray-800">Assigned Queues</h2>
                        <button id="edit-queues-link" class="text-sm font-medium text-blue-600 hover:text-blue-800 pulse-glow">Edit Queues</button>
                    </div>
                    <div id="queues-grid" class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-4"></div>
                </div>

                <!-- Right Column (Info & Skills) -->
                <div class="lg:col-span-1 flex flex-col gap-6">
                    <div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm">
                        <h2 class="text-xl font-semibold text-gray-800 mb-4">Basic Information</h2>
                        <div class="bg-gray-50 rounded-lg p-4 border border-gray-200">
                            <ul id="basic-info-list" class="space-y-3 text-sm"></ul>
                        </div>
                    </div>
                    <div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm">
                        <div class="flex justify-between items-center mb-4">
                            <h2 class="text-xl font-semibold text-gray-800">Skills</h2>
                            <button id="edit-skills-link" class="text-sm font-medium text-blue-600 hover:text-blue-800 pulse-glow">Edit Skills</button>
                        </div>
                        <div class="bg-gray-50 rounded-lg border border-gray-200">
                            <ul id="skills-list" class="divide-y divide-gray-200"></ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- PAGE 2: Skills Editor View (Initially Hidden) -->
        <div id="page-skills-editor" class="hidden">
            <div class="bg-white rounded-lg border border-gray-200 shadow-sm overflow-hidden">
                <div class="p-6 border-b border-gray-200"><h1 id="skills-editor-header" class="text-3xl font-bold text-gray-900"></h1></div>
                <div class="p-6">
                    <div class="grid grid-cols-1 lg:grid-cols-[1fr_auto_1fr] gap-6 items-start">
                        <div class="w-full flex flex-col"><h2 class="text-lg font-semibold text-gray-800 mb-3">Available Skills</h2><div class="flex gap-2 mb-3"><input type="text" id="skills-search-input" placeholder="Search skills..." class="px-4 py-2 border rounded-md w-full text-sm"><button id="skills-search-button" class="px-4 py-2 bg-blue-600 text-white rounded-md text-sm font-semibold hover:bg-blue-700">SEARCH</button></div><div class="border rounded-lg overflow-hidden flex-grow"><table class="min-w-full divide-y divide-gray-200 table-fixed"><thead class="table-header"><tr><th scope="col" class="p-3 w-12"><input type="checkbox" id="selectAllAvailableSkills" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-1/2">Skill</th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-1/2">Description</th></tr></thead><tbody id="available-skills-body"></tbody></table><div id="available-skills-empty-state" class="hidden p-8 text-center text-gray-500"><p></p></div></div><div id="available-skills-pagination" class="mt-4"></div></div>
                        <div class="flex lg:flex-col justify-center items-center gap-3 my-4 lg:my-0 mx-auto pt-20"><button id="add-skill-button" class="w-full lg:w-auto p-3 flex items-center justify-center gap-2 rounded-md border border-gray-300 bg-white text-sm font-medium text-gray-700 hover:bg-gray-50"><svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd" /></svg>Add</button><button id="remove-skill-button" class="w-full lg:w-auto p-3 flex items-center justify-center gap-2 rounded-md border border-gray-300 bg-white text-sm font-medium text-gray-700 hover:bg-gray-50"><svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M12.707 5.293a1 1 0 010 1.414L9.414 10l3.293 3.293a1 1 0 01-1.414 1.414l-4-4a1 1 0 010-1.414l4-4a1 1 0 011.414 0z" clip-rule="evenodd" /></svg>Remove</button></div>
                        <div class="w-full flex flex-col"><h2 class="text-lg font-semibold text-gray-800 mb-3">Assigned Skills</h2><div class="border rounded-lg overflow-hidden flex-grow"><table class="min-w-full divide-y divide-gray-200 table-fixed"><thead class="table-header"><tr><th scope="col" class="p-3 w-12"><input type="checkbox" id="selectAllAssignedSkills" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-1/2">Skill</th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-1/2">Description</th></tr></thead><tbody id="assigned-skills-body"></tbody></table><div id="assigned-skills-empty-state" class="hidden p-8 text-center text-gray-500"><p>None Selected</p></div></div><div id="assigned-skills-pagination" class="mt-4"></div></div>
                    </div>
                </div>
                <div class="p-6 bg-white"><hr class="mb-6 border-gray-200"><div class="flex justify-between items-center"><button id="cancel-skills-button" class="px-6 py-2 border border-gray-300 text-gray-700 rounded-md text-sm font-semibold hover:bg-gray-50">CANCEL</button><button id="save-skills-button" class="px-6 py-2 bg-blue-600 text-white rounded-md text-sm font-semibold hover:bg-blue-700">SAVE</button></div></div>
            </div>
        </div>
        
        <!-- PAGE 3: Queues Editor View (Initially Hidden) -->
        <div id="page-queues-editor" class="hidden">
            <div class="bg-white rounded-lg border border-gray-200 shadow-sm overflow-hidden">
                <div class="p-6 border-b border-gray-200"><h1 id="queues-editor-header" class="text-3xl font-bold text-gray-900"></h1></div>
                <div class="p-6">
                    <div class="grid grid-cols-1 lg:grid-cols-[1fr_auto_1fr] gap-6 items-start">
                        <div class="w-full flex flex-col"><h2 class="text-lg font-semibold text-gray-800 mb-3">Available Queues</h2><div class="flex gap-2 mb-3"><input type="text" id="queues-search-input" placeholder="Search queues..." class="px-4 py-2 border rounded-md w-full text-sm"><button id="queues-search-button" class="px-4 py-2 bg-blue-600 text-white rounded-md text-sm font-semibold hover:bg-blue-700">SEARCH</button></div><div class="border rounded-lg overflow-hidden flex-grow"><table class="min-w-full divide-y divide-gray-200 table-fixed"><thead class="table-header"><tr><th scope="col" class="p-3 w-12"><input type="checkbox" id="selectAllAvailableQueues" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-2/5">Queue</th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-2/5">Description</th><th scope="col" class="p-3 text-center text-xs font-medium text-gray-500 uppercase tracking-wider w-1/5">Skills?</th></tr></thead><tbody id="available-queues-body"></tbody></table><div id="available-queues-empty-state" class="hidden p-8 text-center text-gray-500"><p></p></div></div><div id="available-queues-pagination" class="mt-4"></div></div>
                        <div class="flex lg:flex-col justify-center items-center gap-3 my-4 lg:my-0 mx-auto pt-20"><button id="add-queue-button" class="w-full lg:w-auto p-3 flex items-center justify-center gap-2 rounded-md border border-gray-300 bg-white text-sm font-medium text-gray-700 hover:bg-gray-50"><svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd" /></svg>Add</button><button id="remove-queue-button" class="w-full lg:w-auto p-3 flex items-center justify-center gap-2 rounded-md border border-gray-300 bg-white text-sm font-medium text-gray-700 hover:bg-gray-50"><svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M12.707 5.293a1 1 0 010 1.414L9.414 10l3.293 3.293a1 1 0 01-1.414 1.414l-4-4a1 1 0 010-1.414l4-4a1 1 0 011.414 0z" clip-rule="evenodd" /></svg>Remove</button></div>
                        <div class="w-full flex flex-col"><h2 class="text-lg font-semibold text-gray-800 mb-3">Assigned Queues</h2><div class="flex items-center gap-2 mb-3"><label for="bulk-effective-date" class="text-sm font-medium text-gray-700 whitespace-nowrap">Set all to:</label><input type="date" id="bulk-effective-date" class="px-2 py-1 border rounded-md w-full text-sm"><button id="bulk-set-date-button" class="px-4 py-1.5 bg-gray-200 text-gray-700 rounded-md text-sm font-semibold hover:bg-gray-300">SET</button></div><div class="border rounded-lg overflow-hidden flex-grow"><table class="min-w-full divide-y divide-gray-200 table-fixed"><thead class="table-header"><tr><th scope="col" class="p-3 w-12"><input type="checkbox" id="selectAllAssignedQueues" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-1/3">Queue</th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-1/3">Skills?</th><th scope="col" class="p-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider w-1/3">Effective Date</th></tr></thead><tbody id="assigned-queues-body"></tbody></table><div id="assigned-queues-empty-state" class="hidden p-8 text-center text-gray-500"><p>None Selected</p></div></div><div id="assigned-queues-pagination" class="mt-4"></div></div>
                    </div>
                </div>
                <div class="p-6 bg-white"><hr class="mb-6 border-gray-200"><div class="flex justify-between items-center"><button id="cancel-queues-button" class="px-6 py-2 border border-gray-300 text-gray-700 rounded-md text-sm font-semibold hover:bg-gray-50">CANCEL</button><button id="save-queues-button" class="px-6 py-2 bg-blue-600 text-white rounded-md text-sm font-semibold hover:bg-blue-700">SAVE</button></div></div>
            </div>
        </div>
    </div>

<script>
(function() {
    // --- GLOBAL STATE & DATA ---
    const userInfo = { username: 'James Smith', role: 'LTE', location: 'Off-Shore', createdOn: '12/22/2023 12:18 PM', assignedPeople: 'Mary Anne' };
    const MOCK_CURRENT_DATE = new Date('2025-07-24T15:29:00-04:00');
    
    const allSkills = [
        { id: 1, name: 'Address Lookups', description: 'Can use external tool XYZ to perform address lookups.' },
        { id: 2, name: 'Applicant Communication', description: 'Proficient in effectively communicating with applicants.' },
        { id: 3, name: 'Creole', description: 'Associate is fluent in Haitian Creole.' },
        { id: 4, name: 'Medicare - Enrollee Address Validation', description: 'Specialized in verifying Enrollee addresses.' },
        { id: 5, name: 'P.O. Box Validation', description: 'Proficient in identifying address P.O. Box errors.' },
        { id: 6, name: 'Spanish', description: 'Team member possesses high-degree of fluency in Spanish.' },
        { id: 7, name: 'Cloud Management', description: 'Manages cloud infrastructure and services.' },
        { id: 8, name: 'Data Analysis', description: 'Analyzes data to provide actionable insights.' },
        { id: 9, name: 'AI Development', description: 'Builds and deploys machine learning models.' },
        { id: 10, name: 'Network Engineering', description: 'Designs and maintains network infrastructure.' },
    ];
    let allQueues = [
        { id: 1, name: 'Creole Speakers for Partner DEF', hasRequiredSkills: true, effectiveDate: '2024-01-30', description: 'Handles inquiries from Creole-speaking partners.' },
        { id: 2, name: 'Florida Region 5', hasRequiredSkills: true, effectiveDate: '2024-01-08', description: 'Manages all cases originating from Florida Region 5.' },
        { id: 3, name: 'Healthpilot Technologies LLC', hasRequiredSkills: true, effectiveDate: '2025-08-01', description: 'Dedicated queue for a high-value technology partner.' },
        { id: 4, name: 'NH Customers', hasRequiredSkills: false, effectiveDate: '2024-02-01', description: 'General customer service queue for New Hampshire.' },
        { id: 5, name: 'SEP Election PO Box Errors', hasRequiredSkills: true, effectiveDate: '2025-09-15', description: 'Resolves errors related to P.O. boxes for SEP elections.' },
        { id: 6, name: 'SEP Elections Std. Add. Error', hasRequiredSkills: false, effectiveDate: '2024-01-23', description: 'Handles standard address errors for SEP elections.' },
        { id: 7, name: 'General Inquiries', hasRequiredSkills: true, effectiveDate: '2023-12-01', description: 'Catch-all for general questions and support tickets.' },
        { id: 8, name: 'High Priority Escalations', hasRequiredSkills: true, effectiveDate: '2023-12-01', description: 'For urgent issues requiring immediate attention.' },
        { id: 9, name: 'Partner Onboarding', hasRequiredSkills: false, effectiveDate: '2025-10-05', description: 'Assists new partners with the setup process.' },
        { id: 10, name: 'Billing & Payments', hasRequiredSkills: true, effectiveDate: '2023-11-15', description: 'Handles all billing-related questions and disputes.' },
    ];
    let assignedSkillIds = new Set([1, 2, 3, 4, 5, 6]);
    let assignedQueueIds = new Set([1, 2, 3, 4, 5, 6]);
    
    // --- DOM ELEMENTS ---
    const pageProfile = document.getElementById('page-profile');
    const pageSkillsEditor = document.getElementById('page-skills-editor');
    const pageQueuesEditor = document.getElementById('page-queues-editor');
    
    // --- UTILITY ---
    const getTodayDateString = () => new Date().toISOString().split('T')[0];

    // --- NAVIGATION ---
    function showPage(pageToShow) {
        [pageProfile, pageSkillsEditor, pageQueuesEditor].forEach(page => page.classList.add('hidden'));
        pageToShow.classList.remove('hidden');
    }
    
    // --- PROFILE PAGE ---
    function renderProfilePage() {
        document.getElementById('user-header').textContent = userInfo.username;
        document.getElementById('basic-info-list').innerHTML = `<li class="flex justify-between"><span class="font-medium text-gray-600">Role</span><span class="text-gray-900">${userInfo.role}</span></li><li class="flex justify-between"><span class="font-medium text-gray-600">Location</span><span class="text-gray-900">${userInfo.location}</span></li><li class="flex justify-between"><span class="font-medium text-gray-600">Created On</span><span class="text-gray-900">${userInfo.createdOn}</span></li><li class="flex justify-between"><span class="font-medium text-gray-600">Reports To</span><span class="text-gray-900">${userInfo.assignedPeople}</span></li>`;
        
        const queuesGrid = document.getElementById('queues-grid');
        queuesGrid.innerHTML = '';
        allQueues.filter(q => assignedQueueIds.has(q.id)).forEach(queue => {
            const queueDate = new Date(queue.effectiveDate);
            const isActive = queueDate <= MOCK_CURRENT_DATE;
            const colorClass = isActive ? 'bg-green-500' : 'bg-yellow-400';
            const statusText = isActive ? 'Active' : 'Pending';
            
            const skillStatus = queue.hasRequiredSkills ? `<div class="flex items-center gap-1.5 text-green-600"><svg class="h-4 w-4" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" /></svg><span>Skills Met</span></div>` : `<div class="flex items-center gap-1.5 text-red-600"><svg class="h-4 w-4" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd" /></svg><span>Skills Missing</span></div>`;
            queuesGrid.innerHTML += `<div class="bg-gray-50 rounded-lg border border-gray-200 p-4 flex flex-col justify-between hover:shadow-md transition-shadow"><div><div class="flex justify-between items-start"><h3 class="font-semibold text-gray-900 mb-2">${queue.name}</h3><button class="text-gray-400 hover:text-gray-600"><svg class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor"><path d="M10 6a2 2 0 110-4 2 2 0 010 4zM10 12a2 2 0 110-4 2 2 0 010 4zM10 18a2 2 0 110-4 2 2 0 010 4z" /></svg></button></div><div class="flex items-center gap-2 text-xs text-gray-500 mb-3"><span class="h-2 w-2 rounded-full ${colorClass}"></span><span>${statusText}</span><span>(Eff. ${queue.effectiveDate})</span></div></div><div class="text-xs font-medium">${skillStatus}</div></div>`;
        });

        const skillsList = document.getElementById('skills-list');
        skillsList.innerHTML = '';
        const currentAssignedSkills = allSkills.filter(s => assignedSkillIds.has(s.id));
        if (currentAssignedSkills.length === 0) {
            skillsList.innerHTML = `<li class="p-3 text-sm text-gray-500">No skills assigned.</li>`;
        } else {
            currentAssignedSkills.forEach(skill => {
                skillsList.innerHTML += `<li class="p-3 flex items-center text-sm"><p class="font-medium text-gray-800">${skill.name}</p></li>`;
            });
        }
    }

    // --- GENERIC EDITOR LOGIC ---
    function setupEditor(config) {
        let editorState = { available: [], assigned: [], searchTerm: '', currentPage: 1 };
        
        function initialize() {
            document.getElementById(config.headerId).textContent = `Edit ${userInfo.username}'s ${config.title}`;
            editorState.available = config.allData.filter(item => !config.assignedIds.has(item.id));
            editorState.assigned = config.allData.filter(item => config.assignedIds.has(item.id));
            editorState.searchTerm = '';
            document.getElementById(config.searchInputId).value = '';
            editorState.currentPage = 1;
            render();
        }

        function render() {
            const filteredAvailable = editorState.available.filter(item => config.filterFn(item, editorState.searchTerm));
            renderPicker(document.getElementById(config.availableBodyId), document.getElementById(config.availablePaginationId), document.getElementById(config.availableEmptyId), filteredAvailable, editorState.currentPage, (page) => { editorState.currentPage = page; render(); }, config.availableRowFn, editorState.searchTerm);
            renderPicker(document.getElementById(config.assignedBodyId), document.getElementById(config.assignedPaginationId), document.getElementById(config.assignedEmptyId), editorState.assigned, 1, ()=>{}, config.assignedRowFn, '');
        }
        
        function renderPicker(body, pagination, emptyState, items, currentPage, onPageChange, rowFn, searchTerm) {
            body.innerHTML = '';
            const totalItems = items.length;
            const totalPages = Math.ceil(totalItems / 10);
            if (currentPage > totalPages && totalPages > 0) currentPage = totalPages;
            const pageItems = items.slice((currentPage - 1) * 10, currentPage * 10);
            
            if (pageItems.length > 0) {
                pageItems.forEach(item => body.appendChild(rowFn(item)));
                body.closest('.border').classList.remove('hidden');
                emptyState.classList.add('hidden');
            } else {
                body.closest('.border').classList.add('hidden');
                emptyState.classList.remove('hidden');
                emptyState.querySelector('p').textContent = searchTerm ? `No ${config.title.toLowerCase()} match your search.` : `No available ${config.title.toLowerCase()}.`;
            }
            
            pagination.innerHTML = '';
            if (totalItems <= 10) return;
            const startItem = (currentPage - 1) * 10 + 1;
            const endItem = Math.min(currentPage * 10, totalItems);
            pagination.innerHTML = `<div class="flex items-center justify-between"><p class="text-sm text-gray-700">Showing <span class="font-medium">${startItem}</span> to <span class="font-medium">${endItem}</span> of <span class="font-medium">${totalItems}</span></p></div>`;
        }

        function moveItems(source, dest, bodyId) {
            const selectedIds = new Set(Array.from(document.getElementById(bodyId).querySelectorAll('input:checked')).map(cb => parseInt(cb.dataset.id)));
            if (selectedIds.size === 0) return [source, dest];
            const toMove = source.filter(item => selectedIds.has(item.id));
            const newSource = source.filter(item => !selectedIds.has(item.id));
            dest.push(...toMove);
            dest.sort((a, b) => a.id - b.id);
            return [newSource, dest];
        }

        document.getElementById(config.addButtonId).onclick = () => { 
            const oldDestIds = new Set(editorState.assigned.map(i => i.id));
            [editorState.available, editorState.assigned] = moveItems(editorState.available, editorState.assigned, config.availableBodyId); 
            if (config.onAdd) {
                const newlyAdded = editorState.assigned.filter(i => !oldDestIds.has(i.id));
                config.onAdd(newlyAdded);
            }
            render(); 
        };
        document.getElementById(config.removeButtonId).onclick = () => { 
            [editorState.assigned, editorState.available] = moveItems(editorState.assigned, editorState.available, config.assignedBodyId); 
            render(); 
        };
        document.getElementById(config.searchButtonId).onclick = () => { editorState.searchTerm = document.getElementById(config.searchInputId).value.toLowerCase(); editorState.currentPage = 1; render(); };
        document.getElementById(config.searchInputId).onkeyup = (e) => { if (e.key === 'Enter') document.getElementById(config.searchButtonId).click(); };
        document.getElementById(config.saveButtonId).onclick = () => { config.onSave(new Set(editorState.assigned.map(item => item.id)), editorState.assigned); showPage(pageProfile); };
        document.getElementById(config.cancelButtonId).onclick = () => showPage(pageProfile);
        document.getElementById(config.selectAllAvailableId).onchange = (e) => { document.getElementById(config.availableBodyId).querySelectorAll('input[type="checkbox"]').forEach(cb => cb.checked = e.target.checked); };
        document.getElementById(config.selectAllAssignedId).onchange = (e) => { document.getElementById(config.assignedBodyId).querySelectorAll('input[type="checkbox"]').forEach(cb => cb.checked = e.target.checked); };
        
        if (config.bulkButtonId) {
            document.getElementById(config.bulkButtonId).onclick = () => {
                const newDate = document.getElementById(config.bulkInputId).value;
                if (newDate) {
                    editorState.assigned.forEach(item => item.effectiveDate = newDate);
                    render();
                }
            };
        }

        return { initialize, editorState, render };
    }

    // --- INITIALIZE EDITORS ---
    const skillsEditor = setupEditor({
        page: pageSkillsEditor, title: 'Skills', headerId: 'skills-editor-header', allData: allSkills, assignedIds: assignedSkillIds,
        searchInputId: 'skills-search-input', searchButtonId: 'skills-search-button',
        availableBodyId: 'available-skills-body', assignedBodyId: 'assigned-skills-body',
        availablePaginationId: 'available-skills-pagination', assignedPaginationId: 'assigned-skills-pagination',
        availableEmptyId: 'available-skills-empty-state', assignedEmptyId: 'assigned-skills-empty-state',
        addButtonId: 'add-skill-button', removeButtonId: 'remove-skill-button',
        saveButtonId: 'save-skills-button', cancelButtonId: 'cancel-skills-button',
        selectAllAvailableId: 'selectAllAvailableSkills', selectAllAssignedId: 'selectAllAssignedSkills',
        filterFn: (item, term) => item.name.toLowerCase().includes(term) || item.description.toLowerCase().includes(term),
        availableRowFn: (item) => { const tr = document.createElement('tr'); tr.className = 'table-row'; tr.dataset.id = item.id; tr.innerHTML = `<td class="p-3"><input type="checkbox" data-id="${item.id}" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></td><td class="p-3 break-words">${item.name}</td><td class="p-3 break-words">${item.description}</td>`; return tr; },
        assignedRowFn: (item) => { const tr = document.createElement('tr'); tr.className = 'table-row'; tr.dataset.id = item.id; tr.innerHTML = `<td class="p-3"><input type="checkbox" data-id="${item.id}" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></td><td class="p-3 break-words">${item.name}</td><td class="p-3 break-words">${item.description}</td>`; return tr; },
        onSave: (newIds) => { assignedSkillIds = newIds; renderProfilePage(); }
    });
    
    const queuesEditor = setupEditor({
        page: pageQueuesEditor, title: 'Queues', headerId: 'queues-editor-header', allData: allQueues, assignedIds: assignedQueueIds,
        searchInputId: 'queues-search-input', searchButtonId: 'queues-search-button',
        availableBodyId: 'available-queues-body', assignedBodyId: 'assigned-queues-body',
        availablePaginationId: 'available-queues-pagination', assignedPaginationId: 'assigned-queues-pagination',
        availableEmptyId: 'available-queues-empty-state', assignedEmptyId: 'assigned-queues-empty-state',
        addButtonId: 'add-queue-button', removeButtonId: 'remove-queue-button',
        saveButtonId: 'save-queues-button', cancelButtonId: 'cancel-queues-button',
        selectAllAvailableId: 'selectAllAvailableQueues', selectAllAssignedId: 'selectAllAssignedQueues',
        bulkButtonId: 'bulk-set-date-button', bulkInputId: 'bulk-effective-date',
        filterFn: (item, term) => item.name.toLowerCase().includes(term) || item.description.toLowerCase().includes(term),
        availableRowFn: (item) => { 
            const tr = document.createElement('tr'); tr.className = 'table-row'; tr.dataset.id = item.id;
            const skillIcon = item.hasRequiredSkills ? `<svg class="h-5 w-5 text-green-500" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" /></svg>` : `<svg class="h-5 w-5 text-red-500" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd" /></svg>`;
            tr.innerHTML = `<td class="p-3"><input type="checkbox" data-id="${item.id}" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></td><td class="p-3 break-words">${item.name}</td><td class="p-3 break-words">${item.description}</td><td class="p-3 flex justify-center">${skillIcon}</td>`; 
            return tr; 
        },
        assignedRowFn: (item) => {
            const tr = document.createElement('tr'); tr.className = 'table-row'; tr.dataset.id = item.id;
            const skillIcon = item.hasRequiredSkills ? `<svg class="h-5 w-5 text-green-500" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" /></svg>` : `<svg class="h-5 w-5 text-red-500" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd" /></svg>`;
            tr.innerHTML = `<td class="p-3"><input type="checkbox" data-id="${item.id}" class="h-4 w-4 rounded border-gray-300 custom-checkbox"></td><td class="p-3 break-words">${item.name}</td><td class="p-3 flex justify-center">${skillIcon}</td><td class="p-2"><input type="date" value="${item.effectiveDate}" onchange="this.closest('.table-row').__item.effectiveDate = this.value" class="px-2 py-1 border rounded-md w-full text-sm"></td>`; 
            tr.__item = item; // Attach item data to the element for easy access
            return tr;
        },
        onAdd: (newlyAdded) => {
            newlyAdded.forEach(item => item.effectiveDate = getTodayDateString());
        },
        onSave: (newIds, assignedItems) => { 
            assignedQueueIds = newIds; 
            // Update master list with new dates
            assignedItems.forEach(editedItem => {
                const masterItem = allQueues.find(q => q.id === editedItem.id);
                if (masterItem) masterItem.effectiveDate = editedItem.effectiveDate;
            });
            renderProfilePage(); 
        }
    });

    // --- EVENT LISTENERS ---
    document.addEventListener('DOMContentLoaded', () => {
        document.getElementById('edit-skills-link').addEventListener('click', () => { skillsEditor.initialize(); showPage(pageSkillsEditor); });
        document.getElementById('edit-queues-link').addEventListener('click', () => { queuesEditor.initialize(); showPage(pageQueuesEditor); });
        
        renderProfilePage();
        showPage(pageProfile);
    });
})();
</script>

</body>
</html>
